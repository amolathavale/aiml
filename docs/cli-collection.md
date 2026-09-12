# gcloud CLI Code Blocks


### Create dataproc cluster

```zsh
gcloud config set dataproc/region Region
gcloud services disable dataproc.googleapis.com --force
gcloud services enable dataproc.googleapis.com

PROJECT_ID=$(gcloud config get-value project) && gcloud config set project $PROJECT_ID

PROJECT_NUMBER=$(gcloud projects describe $PROJECT_ID --format='value(projectNumber)')

gcloud projects add-iam-policy-binding $PROJECT_ID \
  --member=serviceAccount:$PROJECT_NUMBER-compute@developer.gserviceaccount.com \
  --role=roles/storage.admin

gcloud projects add-iam-policy-binding $PROJECT_ID \
  --member=serviceAccount:$PROJECT_NUMBER-compute@developer.gserviceaccount.com \
  --role=roles/dataproc.worker

gcloud compute networks subnets update default --region=REGION  --enable-private-ip-google-access

gcloud dataproc clusters create example-cluster --worker-boot-disk-size 500 --worker-machine-type=e2-standard-4 --master-machine-type=e2-standard-4

gcloud dataproc clusters update example-cluster --num-workers 4

```

### Submit a job

```zsh
gcloud dataproc jobs submit spark --cluster example-cluster \
  --class org.apache.spark.examples.SparkPi \
  --jars file:///usr/lib/spark/examples/jars/spark-examples.jar -- 1000

```

### IAM / Config / Setup related
```zsh
gcloud auth list
gcloud config list project
export GOOGLE_CLOUD_PROJECT=$(gcloud config get-value core/project)
gcloud iam service-accounts create my-natlang-sa --display-name "my natural language service account"
gcloud iam service-accounts keys create ~/key.json --iam-account my-natlang-sa@${GOOGLE_CLOUD_PROJECT}.iam.gserviceaccount.com
export GOOGLE_APPLICATION_CREDENTIALS="/home/USER/key.json"
gcloud iam service-accounts create quickstart
gcloud iam service-accounts keys create key.json --iam-account quickstart@<your-project-123>.iam.gserviceaccount.com
gcloud auth activate-service-account --key-file key.json
gcloud auth print-access-token
gcloud beta services identity create --service=dataprep.googleapis.com
```

### Dataflow
```zsh
gcloud services disable dataflow.googleapis.com --project Project ID --force
gcloud services enable dataflow.googleapis.com --project Project ID
gcloud storage cp -r gs://spls/gsp290/dataflow-python-examples .
gcloud storage buckets create gs://BUCKET_NAME --location=REGION
gcloud storage cp gs://spls/gsp290/data_files/usa_names.csv gs://BUCKET_NAME/data_files/
gcloud storage cp gs://spls/gsp290/data_files/head_usa_names.csv gs://BUCKET_NAME/data_files/

bq mk lake

pip install apache-beam[gcp]==2.59.0

python dataflow_python_examples/data_ingestion.py \
  --project=PROJECT_ID \
  --region=REGION \
  --runner=DataflowRunner \
  --machine_type=e2-standard-2 \
  --staging_location=gs://BUCKET_NAME/test \
  --temp_location gs://BUCKET_NAME/test \
  --input gs://BUCKET_NAME/data_files/head_usa_names.csv \
  --save_main_session

python dataflow_python_examples/data_transformation.py \
  --project=PROJECT_ID \
  --region=REGION \
  --runner=DataflowRunner \
  --machine_type=e2-standard-2 \
  --staging_location=gs://BUCKET_NAME/test \
  --temp_location gs://BUCKET_NAME/test \
  --input gs://BUCKET_NAME/data_files/head_usa_names.csv \
  --save_main_session

python dataflow_python_examples/data_enrichment.py \
  --project=PROJECT_ID \
  --region=REGION \
  --runner=DataflowRunner \
  --machine_type=e2-standard-2 \
  --staging_location=gs://BUCKET_NAME/test \
  --temp_location gs://BUCKET_NAME/test \
  --input gs://BUCKET_NAME/data_files/head_usa_names.csv \
  --save_main_session

python dataflow_python_examples/data_lake_to_mart.py \
  --worker_disk_type="compute.googleapis.com/projects//zones//diskTypes/pd-ssd" \
  --max_num_workers=4 \
  --project=PROJECT_ID \
  --runner=DataflowRunner \
  --machine_type=e2-standard-2 \
  --staging_location=gs://BUCKET_NAME/test \
  --temp_location gs://BUCKET_NAME/test \
  --save_main_session \
  --region=REGION


```

### NLP APIs
```zsh
gcloud ml language analyze-entities --content="Michelangelo Caravaggio, Italian painter, is known for 'The Calling of Saint Matthew'." > result.json

cat result.json
```

### Speech-to-Text APIs
```zsh
cat << EoF > ./request.json
{
  "config": {
      "encoding":"FLAC",
      "languageCode": "en-US"
  },
  "audio": {
      "uri":"gs://cloud-samples-tests/speech/brooklyn.flac"
  }
}
EoF

curl -s -X POST -H "Content-Type: application/json" --data-binary @request.json \
"https://speech.googleapis.com/v1/speech:recognize?key=${API_KEY}"

curl -s -X POST -H "Content-Type: application/json" --data-binary @request.json \
"https://speech.googleapis.com/v1/speech:recognize?key=${API_KEY}" > result.json
```


### Video Intelligence APIs
```zsh
cat > request.json <<EOF
{
   "inputUri":"gs://spls/gsp154/video/train.mp4",
   "features": [
       "LABEL_DETECTION"
   ]
}
EOF

curl -s -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer '$(gcloud auth print-access-token)'' \
    'https://videointelligence.googleapis.com/v1/videos:annotate' \
    -d @request.json

curl -s -H 'Content-Type: application/json' \
    -H 'Authorization: Bearer '$(gcloud auth print-access-token)'' \
    'https://videointelligence.googleapis.com/v1/projects/PROJECTS/locations/LOCATIONS/operations/OPERATION_NAME'
```

### Github repo with all GCP PDE/PMLE labs
```zsh
git clone https://github.com/GoogleCloudPlatform/training-data-analyst
git clone https://github.com/GoogleCloudPlatform/asl-ml-immersion.git 
```