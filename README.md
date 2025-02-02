🚀 Network Phishing Website Detection Using Machine Learning and MLOps

This project focuses on detecting phishing websites using Machine Learning (ML) and MLOps. It includes a complete deployment pipeline on AWS EC2 and ECR, demonstrating the end-to-end workflow of building and deploying a machine learning model for phishing website detection.

📖 Table of Contents

•	Project Overview

•	Architecture

•	Components
  - Data Ingestion
  - Data Validation
  - Data Transformation
  - Model Training
  - Model Deployment
  - CI/CD Pipeline
    
•	Technologies Used

🛠 Project Overview

This project aims to create a robust pipeline for detecting phishing websites using machine learning. It covers essential aspects of MLOps, such as data ingestion, validation, transformation, model training, deployment, and continuous integration/continuous deployment (CI/CD). The complete deployment pipeline is implemented on AWS EC2 and ECR.



🏗️ Architecture

The project uses a modular approach for data processing, model training, and deployment. The architecture includes components such as data ingestion, validation, transformation, and model deployment with automated CI/CD integration.



🔧 Components

📥 Data Ingestion

Script: push_data.py, data_ingenstion.py
Function: Reads phishing data from CSV, converts it to JSON format, and stores it in MongoDB.


🛡️ Data Validation

Script: data_validation.py
Function: Ensures dataset quality, performs schema validation, and detects dataset drift.


🔄 Data Transformation

Script: data_transformation.py
Function: Applies KNN imputer for handling missing values and prepares datasets for ML training.


🧑‍💻 Model Training

Script: model_trainer.py
Function: Trains multiple machine learning models, evaluates them, and tracks experiments using MLflow.


🚀 Model Deployment

Script: app.py
Function: Deploys the trained model using FastAPI for serving predictions on new data.


🔄 CI/CD Pipeline
Workflow File: .github/workflows/main.yml
Function: Automates deployment using GitHub Actions, Docker, AWS ECR, and EC2 for continuous integration and deployment.



🛠 Technologies Used:

🐍 Python: Programming language used for the project.

📊 Machine Learning Libraries: Pandas, NumPy, Scikit-learn for data processing and model training.

🗃️ MongoDB: NoSQL database for storing phishing data.

⚡ FastAPI: Framework used for building APIs to serve predictions.

🐳 Docker: Containerization for easy deployment of the model.

🔧 GitHub Actions: Automates CI/CD workflow.

☁️ AWS: EC2 for deployment, ECR for storing Docker images, and S3 for cloud storage.

📈 MLflow: For experiment tracking and model management.
