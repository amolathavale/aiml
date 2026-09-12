# 100 DAY Uplift Plan

Pro-Tips for Daily Execution (2–3 Hours/Day)
Time Allocation: Spend the first 30–45 minutes reviewing concepts or reading documentation, and dedicate the remaining 1.5–2 hours entirely to writing code, debugging errors, and building.
Consistency over Intensity: Daily small progress compounds significantly more than weekend-only cramming.
Public Sharing: Push all your hands-on code scripts and daily exercises to GitHub to build immediate social proof.

---
## Phase 1: Advanced SQL & High-Performance Data Manipulation (#### Days 1–20)
Moving beyond basic SELECT statements to complex analytical queries and efficient Pandas workflows.

#### Days 1–5: Advanced SQL for Data Science
Task: Practice window functions (`ROW_NUMBER()`, `RANK()`, `LAG()`, `LEAD()`) and CTEs on platforms like LeetCode or Stratascratch.
Hands-on: Write a query calculating rolling 7-day active user averages and user retention cohorts.
#### Days 6–10: Database Optimization & Indexing
Task: Learn about indexing, query execution plans, and writing performant joins for large datasets.
Hands-on: Optimize a slow-running SQL query by creating proper indexes and analyzing execution cost.
#### Days 11–15: Advanced Pandas & Vectorization
Task: Master `groupby`, `pivot_table`, multi-indexing, and memory optimization (`pd.Categorical`, chunking large CSVs).
Hands-on: Process a 1GB+ dataset entirely in Pandas without crashing your RAM.
#### Days 16–20: SQL + Python Integration
Task: Use SQLAlchemy and Pandas (`pd.read_sql`) to build data pipelines directly from a local PostgreSQL/MySQL database.
Hands-on: Pull raw transactional data via SQL, transform it using Pandas, and push aggregated results back into a new SQL table.

---
## Phase 2: Exploratory Data Analysis & Feature Engineering (#### Days 21–40)
Real-world data is messy; this ## Phase teaches you how to extract signal from noise.
#### Days 21–25: Advanced Exploratory Data Analysis (EDA)
Task: Use Seaborn and Plotly to uncover deep multi-variate correlations, skewness, and anomalies.
Hands-on: Conduct a full EDA report on a complex dataset (e.g., house prices or telecom churn), identifying at least 3 non-obvious business insights.
#### Days 26–30: Handling Missing Data & Outliers
Task: Implement advanced imputation techniques (KNN Imputer, Iterative Imputer) instead of simple mean/median dropping.
Hands-on: Test different outlier detection methods (Isolation Forest vs. IQR method) and measure their impact on data integrity.
#### Days 31–35: Feature Transformation & Scaling
Task: Master log transforms, Box-Cox, standardization, and robust scaling.
Hands-on: Build custom scikit-learn transformers using `FunctionTransformer` and `Pipeline`.
#### Days 36–40: Advanced Categorical Encoding & Feature Selection
Task: Implement Target Encoding, Frequency Encoding, and Feature Selection via Recursive Feature Elimination (RFE) and Mutual Information.
Hands-on: Reduce a 50-feature dataset down to the top 10 most predictive features without losing model accuracy.

---
## Phase 3: Supervised & Unsupervised Machine Learning (#### Days 41–70)
Moving past default model configurations to rigorous optimization and validation.
#### Days 41–48: Regression & Classification Deep Dive
Task: Build and tune Logistic/Linear Regression, Random Forests, and Support Vector Machines.
Hands-on: Implement cross-validation properly. Never evaluate on training data; strictly use Stratified K-Fold.
#### Days 49–56: Gradient Boosting Mastery (XGBoost, LightGBM, CatBoost)
Task: Understand how boosting works under the hood. Learn key hyperparameters (learning rate, max depth, subsample).
Hands-on: Enter a beginner-friendly tabular competition on Kaggle using LightGBM and build an automated hyperparameter tuning script using Optuna.
#### Days 57–63: Model Evaluation & Debugging
Task: Move past basic "accuracy". Master Precision-Recall curves, ROC-AUC, Log Loss, and Cost Matrices.
Hands-on: Build a model for an imbalanced dataset (e.g., fraud detection) using SMOTE, and optimize specifically for F1-score or Precision at top-k.
#### Days 64–70: Unsupervised Learning & Dimensionality Reduction
Task: Explore K-Means, DBSCAN, Hierarchical Clustering, and Principal Component Analysis (PCA).
Hands-on: Segment a customer database using K-Means and visualize clusters using PCA and t-SNE.

---
## Phase 4: Model Deployment & MLOps Basics (#### Days 71–85)
Bridging the gap between a Jupyter Notebook script and a real-world tool.
#### Days 71–75: Model Serialization & Experiment Tracking
Task: Learn how to save models cleanly using `joblib` or `pickle`. Introduce yourself to MLflow or basic experiment logging.
Hands-on: Track different model iterations, metrics, and parameters for a classification project.
#### Days 76–80: Building APIs with FastAPI
Task: Learn how to wrap a trained machine learning model inside a lightweight web API.
Hands-on: Create a `/predict` endpoint that takes JSON inputs, passes them through your data pipeline, and returns real-time model inferences.
#### Days 81–85: Containerization Basics (Docker)
Task: Understand how to containerize your Python application and model dependencies.
Hands-on: Write a `Dockerfile` that packages your FastAPI app and model file, ensuring it can run seamlessly on any machine.

---
## Phase 5: Capstone Portfolio Projects (#### Days 86–100)
Building 2 production-grade, portfolio-worthy end-to-end projects.
#### Days 86–92: Capstone Project 1 — End-to-End Predictive Modeling
Task: Pick a unique problem (e.g., predicting energy consumption, real estate valuation, or dynamic pricing).
Hands-on: Ingest data via SQL -> Run EDA -> Engineer features -> Train multiple models with Optuna tuning -> Document everything clearly in a professional GitHub repository README.
#### Days 93–99: Capstone Project 2 — End-to-End Analytics & Deployment
Task: Build an application where users input data, a backend SQL/Python script processes it, and a deployed ML model serves predictions via an API or a simple Streamlit dashboard.
Hands-on: Deploy your Streamlit app or FastAPI service to a cloud provider (like Render, Hugging Face Spaces, or Railway).
Day 100: Portfolio Polish & Resume Refinement
Task: Clean up your GitHub profile, pin your top 3 repositories, write clean documentation, and align your resume with your new technical accomplishments.

