# Professional Machine Learning Engineer Certification

A Machine Learning Engineer designs, builds, and productionizes ML systems to solve business challenges. This certification learning path provides the advanced knowledge and practical skills required for this role, preparing you to successfully operate and maintain ML systems on Google Cloud.

Through a curated collection of on-demand courses, labs, and skill badges, you will gain real-world, applied experience with Google Cloud technologies. This path focuses on the essential skills for the ML Engineer role, from designing and building ML systems to optimizing and maintaining them in production.

## Introduction to AI and Machine Learning on Google Cloud
This course introduces Google Cloud's AI and machine learning (ML) capabilities, with a focus on developing both generative and predictive AI projects. It explores the various technologies, products, and tools available throughout the data-to-AI lifecycle, empowering data scientists, AI developers, and ML engineers to enhance their expertise through interactive exercises.

- AI on google cloud
- AI Infrastructure
- AI Models
- BigQuery ML
- [Lab] Predict Visitor Purchases with BigQuery ML
- [Reading](https://partner.skills.google/paths/84/course_templates/593/documents/636903) AI foundations
    - Google Cloud products: Overall, [AI and Machine Learning](https://cloud.google.com/products/ai)
    - Google’s [AI principles](https://ai.google/principles/)
    - Cloud [TPUs](https://cloud.google.com/tpu)
    - AI and ML in BigQuery: [Introduction](https://docs.cloud.google.com/bigquery/docs/bqml-introduction), [SQL syntax](https://docs.cloud.google.com/bigquery/docs/reference/standard-sql/query-syntax)
- Generative AI on Google CLoud
- Foundation Models
- Prompt Engineering
- Deployment and Model Tuning
- Gemini Agent Studio
- AI Agents and building with Google Cloud
- [Reading](https://partner.skills.google/paths/84/course_templates/593/documents/636914) Google gen AI docs:
    - [Generative AI on Vertex AI](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models#overview-of-generative-ai-on-vertex-ai)
    - [Google AI models](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/google-models)
    - [Gemini Enterprise](https://docs.cloud.google.com/gemini/enterprise/docs/get-started)
    - [Introduction to prompting](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/prompts/introduction-prompt-design)
    - [AI and Machine Learning solutions](https://cloud.google.com/solutions/ai)
    - [Agent Development Kit (ADK): Quickstart and tutorials (Google doc)](https://adk.dev/)
    - Google research papers:
    - [Attention is all you need: the Transformer paper](chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://proceedings.neurips.cc/paper_files/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf)
    - [Agents: Google whitepaper](https://drive.google.com/file/d/1W8EnoPXRLTQesfjvb-b3Zj-dnBf1f--n/view)
    - Courses:
    - Create embeddings, vector search, and RAG with BigQuery, YouTube intro video
    - Vector search and embeddings, YouTube intro video
- AI Development options
    - Vertex AI
    - Auto ML
    - Pretrained APIs
    - Custom training
- [Lab] Entity and Sentiment Analysis with the Natural Language API
- [Reading](https://partner.skills.google/paths/84/course_templates/593/documents/636924) AI development options
    - Natural Language API basics
    - AI APIs for Google Cloud
    - Introduction to Vertex AI
    - AutoML: beginner's guide
    - Custom training: beginner's guide
    - Tf.keras documentation
    - Course: Natural Language Processing on Google Cloud
- ML Workflow
- Data Preparation
- Model Development
- Model Serving
- MLOps and workflow automation
- [Lab] Agent Platform - Predicting Loan Risk with AutoML
- How machine learns
- [Reading](https://partner.skills.google/paths/84/course_templates/593/documents/636935) AI development workflow
    - MLOps: overview
    - Introduction to Vertex AI Pipelines
    - Introduction to Vertex Pipelines lab
    - Introduction to Vertex AI SDK
    - Explainable AI
    - Course: Introduction to Vertex Forecasting and Time Series in Practice

## Prepare Data for ML APIs on Google Cloud
- [Lab] Cloud DataPrep - Alteryx Designer Cloud (Trifacta)
Serverless, scalable, intelligent data service for visually exploring, cleaning, and preparing data for analysis, manipulate a dataset, import datasets, correct mismatched data, transform data, and join data
- [Lab] Cloud Dataflow
Create a streaming pipeline using Dataflow, use the Pub/Sub to BigQuery template, which reads messages written in JSON from a Pub/Sub topic and pushes them to a BigQuery table, use the Cloud Shell command line or the Cloud console to create the BigQuery dataset and table, Create a Cloud Storage bucket, Create a streaming pipeline using the Pub/Sub to BigQuery Dataflow template
- [Lab] Cloud Dataflow + Python
Use Apache Beam SDK to define data pipelines, use Dataflow to run your pipeline, set up your Python development environment, Create a Cloud Storage bucket to store results of a Dataflow pipeline, Install the Apache Beam SDK for Python, Run a Dataflow pipeline remotely
- [Lab] Managed Service for Apache Spark
fully-managed cloud service for running Apache Spark and Apache Hadoop clusters, use Google Cloud console or Command Line to create a Managed Apache Spark cluster, run a simple Apache Spark job in the cluster, and then modify the number of workers in the cluster
- [Lab] Cloud Natural Language API: Qwik Start
Natural language processing (NLP) - interaction between computers and human language, enabling computers to understand and process human language in a way that is similar humans. Cloud Natural Language API provides NLP capabilities - analyze text, identify entities, extract information, and answer questions - Entity Recognition, Sentiment Analysis, Information Extraction, Question Answering, Integrated REST API
- [Lab] Speech-to-Text API
Google speech recognition technologies-  send audio and receive a text transcription, Create a Speech-to-Text API request, Call the Speech-to-Text API.
- [Lab] Prepare Data for ML APIs on Google Cloud: Challenge Lab
extend learned skills, changing default values and reading and researching error messages to fix your own mistakes, complete all tasks within the time period : Create a simple Managed Apache Spark job (Cluster+job), Create a simple DataFlow job (GCS->BQ), Perform two Google machine learning backed API tasks

## Create ML Models with BigQuery ML
- [Lab] Getting Started with BigQuery ML
Use available BQ [ecommerce dataset](https://support.google.com/analytics/answer/7586738?hl=en&ref_topic=3416089#zippy=%2Cin-this-article) with millions of Google Analytics records for Google Merchandise Store, create a model that predicts whether a visitor will make a transaction,Create BigQuery datasets, Create, evaluate, and use machine learning models in BigQuery
- [Lab] Predict Visitor Purchases with a Classification Model in BigQuery ML
Use ecommerce dataset above: Use BigQuery to find public datasets, Query and explore the ecommerce dataset, Create a training and evaluation dataset to be used for batch prediction, Create a classification (logistic regression) model in BigQuery ML, Evaluate and improve the performance of your machine learning model, Predict and rank the probability that a visitor will make a purchase
- [Lab] Predict Taxi Fare with a BigQuery ML Forecasting Model
Use BigQuery to find public datasets, Query and explore the public taxi cab dataset, Create a training and evaluation dataset to be used for batch prediction, Create a forecasting (linear regression) model in BigQuery ML, Evaluate the performance of your machine learning model
- [Lab] Bracketology  with BQML-  prototype, train, evaluate, and predict the 'winners' and 'losers' between two NCAA basketball tournament teams, Use BigQuery to access the public NCAA dataset, Explore the  National Collegiate Athletic Association (NCAA) dataset to gain familiarity with the schema and scope of the data available, Prepare and transform the existing data into features and labels, Split the dataset into training and evaluation subsets, Use BigQuery ML to build a model based on the NCAA tournament dataset, Use your newly created model to predict NCAA tournament winners for your bracket

## Engineer Data for Predictive Modeling with BigQuery ML
-[Lab] Creating a Data Transformation Pipeline with Cloud Dataprep
Use ecommerce dataset - Google Analytics session records -  Google Merchandise Store, Explore the available fields and rows and prepare the data for analysis, Connect BigQuery datasets to Dataprep, Explore dataset quality with Dataprep, Create a data transformation pipeline with Dataprep, Run transformation jobs and send outputs to BigQuery
- [Lab] ETL Processing on Google Cloud Using Dataflow and BigQuery (Python)
Apache Beam SDK + Python -> Pipeline -> Cloud Dataflow -> GCS Bucket -> BQ Dataset.Table, then  transform and enrich the data in BigQuery, Ingest data from Cloud Storage to BigQuery, Transform and enrich data in BigQuery, Join data in BigQuery and write the results to a new table


## Production Machine Learning Systems
- implement various flavors of production ML systems - static, dynamic, and continuous training; static and dynamic inference; and batch and online processing
- Delve into TensorFlow abstraction levels, the various options for doing distributed training, and how to write distributed training models with custom estimators.
- advanced ML on GCP, architecting ML systems, Data Extraction, Analysis & preparation, model training, evaluation and validation, trained model, prediction service, performance monitoring, training design decisions, serving design decisions, serving design decisions, designing from scratch, using vertex AI
- adapting to data, changing distributions, right & wrong decisions, system failure, concept drift, actions to mitigate concept drift, TF Data validation, components of TF data validation, advanced data visualisation with TF data validation, mitigating traiing-serving skew through design, diagnosing a production model, 

- [Lab] Agent Platform: Training and Serving a Custom Model
Use Agent Platform to train and serve TensorFlow model using code in a custom container, Build and containerize model training code in Vertex Notebooks, Submit a custom model training job to Agent Platform, Deploy your trained model to an endpoint, and use that endpoint to get predictions

![](https://cdn.qwiklabs.com/49nS%2F5fbsNTZB7qpAw0ZFL%2Byh2qkV7vcDoEzmfKmVkM%3D)

- [Reading] architecting production ML systems
    - [Architecture of a real-world Machine Learning system](https://medium.com/louis-dorard/architecture-of-a-real-world-machine-learning-system-795254bec646)
    - [Machine Learning Pipeline: Architecture of ML Platform in Production](https://www.altexsoft.com/blog/machine-learning-pipeline/)
    - [Production ML systems](https://developers.google.com/machine-learning/crash-course/production-ml-systems)
    - [3 Building Blocks of Machine Learning you Should Know as a Data Scientist](https://www.analyticsvidhya.com/blog/2020/06/3-building-blocks-machine-learning-data-scientist/)
    - [MLOps: Continuous delivery and automation pipelines in machine learning](https://docs.cloud.google.com/architecture/mlops-continuous-delivery-and-automation-pipelines-in-machine-learning)
    - [Smart Decisions Game: Machine Learning for Architects](https://www.sei.cmu.edu/library/smart-decisions-game-machine-learning-for-architects/)
    - [Using TensorFlow to predict product weight and dimensions](https://blog.tensorflow.org/2019/09/using-tensorflow-to-predict-product.html)
    - [Introduction to loading data](https://docs.cloud.google.com/bigquery/docs/loading-data)
    - [Gemini Enterprise Agent Platform](https://cloud.google.com/products/gemini-enterprise-agent-platform)
    - [AI Simplified](https://www.youtube.com/playlist?list=PLIivdWyY5sqJ1YuMdGjRwJ3fFYZ_vWQ62)
    - [AI & Machine Learning](https://cloud.google.com/blog/products/ai-machine-learning)
    - [Google Cloud Pipeline Components](https://github.com/kubeflow/pipelines/tree/master/components/google-cloud#google-cloud-pipeline-components)
    - [Vertex AI:Building a fraud detection model with AutoML](https://codelabs.developers.google.com/vertex-automl-tabular#0)



- Designing high performance ML systems
Distributed training architectures, faster input pipelines, inference, TF distributed training strategies: Mirrorred/Multi-worker mirrorred/TPU/Parameter server, training on large datasets with tf.data API
- [Lab] Distributed Training with Keras
tf.distribute.Strategy API provides an abstraction for distributing training across multiple processing units. uses the tf.distribute.MirroredStrategy, which does in-graph replication with synchronous training on many GPUs on one machine. Essentially, it copies all of the model's variables to each processor. Then, it uses all-reduce to combine the gradients from all processors and applies the combined value to all copies of the model. - Define a distribution strategy and set an input pipeline, Create the Keras model, Define the callbacks, Train and evaluate the model.
- [Reading] Designing High-performance ML Systems
    - [Evaluate Performance of ML Model](https://www.kdnuggets.com/2020/09/performance-machine-learning-model.html)
    - [boost ML Model Performance: Five Ways](https://www.anolytics.ai/blog/how-to-improve-machine-learning-model-performance/)
    - [Distributed TensorFlow model training on Cloud AI Platform](https://www.youtube.com/watch?v=I29_VZ82KW4)
    - [Speeding Up NN Training with Data Echoing](https://research.google/blog/speeding-up-neural-network-training-with-data-echoing/)
    - [ML Performance Improvement Cheat Sheet](https://machinelearningmastery.com/machine-learning-performance-improvement-cheat-sheet/)
    - [Distributed training with TensorFlow](https://www.tensorflow.org/guide/distributed_training)

- Designing Adaptable ML Systems
Adapting to data, changing distributions, Right and Wrong decisions, system failure, concept drift and actions to mitigate, TF data validation- Components: The Statistics Generation component, the Schema Generation component, and the Example Validator component, Advanced visualization with TF data validation, mitigating training-serving skew through design, diagnosing a production model
- [Lab] Agent Platform: Training and Serving a Custom Model
Use Agent Platform to train and serve a TensorFlow model using code in a custom container. Build and containerize model training code in Vertex Notebooks, Submit a custom model training job to Agent Platform, Deploy your trained model to an endpoint, and use that endpoint to get predictions.
- [Reading]  Designing Adaptable ML Systems
    - [Deep Learning AI Needs Tools To Adapt To Changes In The Data Environment](https://www.forbes.com/sites/davidteich/2020/07/16/deep-learning-ai-needs-tools-to-adapt-to-changes-in-the-data-environment/#5c1a6f8c4414)
    - [Machine Learning for Future System Designs](https://www.nextplatform.com/ai/2020/10/29/machine-learning-for-future-system-designs/1644841)
    - [Three Risks in Building Machine Learning Systems](https://www.sei.cmu.edu/blog/three-risks-in-building-machine-learning-systems/)
    - [Adaptive AI vs Traditional AI: What’s the Difference and Why It Matters](https://trinus.com/adaptive-ai-vs-traditional-ai-whats-the-difference-and-why-it-matters/)
    - [ML Opening New Doors For FPGAs](https://semiengineering.com/fpgas-hide-hardware-for-machine-learning/)
    - [Rules of Machine Learning](https://developers.google.com/machine-learning/guides/rules-of-ml)
    - [Productionizing Behavioural Features for Machine Learning with Apache Spark Streaming](https://www.youtube.com/watch?v=cpR6Vkp7ImA)
    - [TensorFlow Data Validation: Checking and analyzing your data](https://www.tensorflow.org/tfx/guide/tfdv)

- Designing Hybrid ML Systems
hybrid cloud machine learning models, Kubeflow, optimize TensorFlow graphs for mobile, TFLight, composability, portability, scalability, 
- [Readings] Hybrid ML Systems
    - [Kubeflow](https://www.kubeflow.org/)
    - [Introduction to Kubeflow](https://www.youtube.com/watch?v=cTZArDgbIWw)
    - [Orchestrating TFX Pipelines](https://www.tensorflow.org/tfx/guide/kubeflow#kubeflow_pipelines)
    - [Introduction to ML Pipelines with Kubeflow](https://www.suse.com/c/rancher_blog/introduction-to-machine-learning-pipelines-with-kubeflow/)
    - [Kubeflow - a ML toolkit for Kubernetes](https://medium.com/@michal.brys/kubeflow-a-machine-learning-toolkit-for-kubernetes-d8686f6c91b6)
    - [LiteRT](https://developers.google.com/edge/litert)
    - [TFLite examples](https://github.com/tensorflow/examples/tree/master/lite/examples)

## Machine Learning Operations (MLOps)
MLOps tools and best practices for deploying, evaluating, monitoring and operating production ML systems on GCP. use tools for continuous improvement and evaluation of deployed models.

### Employing Machine Learning Operations
- MLOps-Why and when to employ MLOps, Machine learning (ML) practitioners' pain points, The concept of devOps in ML, ML Lifecycle, automating ML process
- ML Lifecycle phases
discovery -> development ->  deployment
business use case definition => Data Exploration => Architecture & algorithm selection => Feature engineering & Data pipeline creation => Build ML model => Evaulate => Presentation of results => Plan for deployment => Model Operationalisation =>> Model monitoring

contextual understanding of the people , define the problem or task that needs to be solved, feasiblity of solving with machine learning, Data accessibility and data exploration, Architecture and algorithm selection, Prioritizing use cases, 

- [Reading] 
[Machine Learning: The High Interest Credit Card of Technical Debt](https://research.google/pubs/machine-learning-the-high-interest-credit-card-of-technical-debt/)
[Data preprocessing for ML documentation](https://www.tensorflow.org/tfx/transform/get_started#introduction)
[Documentation - Characteristics of MLOPs](https://docs.cloud.google.com/architecture/mlops-continuous-delivery-and-automation-pipelines-in-machine-learning#characteristics)
[Documentation - Characteristics of MLOps level 2](https://docs.cloud.google.com/architecture/mlops-continuous-delivery-and-automation-pipelines-in-machine-learning#characteristics_3)

### Vertex AI and MLOps on Vertex AI

- GEAP (Vertex AI unified platform), Automate MLOps on Vertex AI, Data Engineering => ML Engineering => App Engineering
Ingest (prepare data) => Analyse and transform (perfrom feature engg) => Train (train & tune mdl) => upload (store and track mdl) => Evaluate (Compare model versions) => Deploy model (to endpoint/s) => Predict (req to endpoint) => Manage endpoints (incl edge devices) => Monitor (and manage the mdl - feature store, model registry, ML Metadata, Eval) 
- rapid setup of ML env, automate process orchestration, manage large infra/storage/network, low latency applications  
Tech stack => GCS, Dataprep, Dataflow, BQ, BQML, GEAP (Custom trg, AutoML, Model Registry/Garden, Batch, Online, Model monitoring, Explainable AI) 

- [Reading]
[Vertex AI documentation](https://docs.cloud.google.com/gemini-enterprise-agent-platform)
[ML metadata artifact types](https://docs.cloud.google.com/gemini-enterprise-agent-platform/machine-learning/pipelines/artifact-types)
[Google Research areas](https://research.google/people/)
[Deepmind Research](https://deepmind.google/research/)
[Publication database](https://research.google/pubs/)
[Towards ML Engineering: A Brief History Of TensorFlow Extended (TFX)](https://arxiv.org/pdf/2010.02013)
[Vertex AI](https://cloud.google.com/products/gemini-enterprise-agent-platform)
[Vertex AI as a pipeline component](https://docs.cloud.google.com/gemini-enterprise-agent-platform/machine-learning/pipelines/model-evaluation-component)
[Choosing between the Kubeflow Pipelines SDK and TFX](https://docs.cloud.google.com/gemini-enterprise-agent-platform/machine-learning/pipelines/build-pipeline#sdk)
[Introduction to Vertex AI Model Monitoring](https://docs.cloud.google.com/gemini-enterprise-agent-platform/machine-learning/model-monitoring/overview)
[Vertex ML Metadata](https://docs.cloud.google.com/gemini-enterprise-agent-platform/machine-learning/ml-metadata/introduction)
[Introduction to Vertex AI Model Monitoring](https://docs.cloud.google.com/gemini-enterprise-agent-platform/machine-learning/model-monitoring/overview)
[Open source TensorBoard](https://www.tensorflow.org/tensorboard/get_started)
[Vertex AI TensorBoard](https://docs.cloud.google.com/gemini-enterprise-agent-platform/machine-learning/experiments/tensorboard-introduction)