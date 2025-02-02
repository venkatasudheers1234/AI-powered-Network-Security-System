Network Phishing Website Detection Using Machine Learning and MLOps.
This project focuses on the detection of phishing websites using Machine Learning and MLOps. The project involves a complete deployment pipeline on AWS EC2 and ECR.
Table of Contents
1. Project Overview
2. Architecture
3. Setup Instructions
4. Components
   -Data Ingestion
   -Data Validation
   -Data Transformation
   -Model Training
   -Model Deployment
   -CI/CD Pipeline
5. Technologies Used

Project Overview
This project aims to create a robust pipeline for detecting phishing websites using machine learning. The project covers all the essential aspects of MLOps, including data ingestion, validation, transformation, model training, deployment, and continuous integration/continuous deployment (CI/CD).

Data Ingestion
Script: push_data.py

Function: Reads phishing data from CSV, converts to JSON, stores in MongoDB.

Data Validation
Script: data_validation.py

Function: Ensures dataset quality, performs schema validation, detects dataset drift.

Data Transformation
Script: data_transformation.py

Function: Applies KNN imputer for missing values, prepares datasets for ML training.

Model Training

Script: model_trainer.py

Function: Trains multiple models, evaluates, and tracks experiments using MLflow.

Model Deployment
Script: app.py

Function: Deploys the model using FastAPI for serving predictions.

CI/CD Pipeline
Workflow File: .github/workflows/main.yml
Function: Automates deployment using GitHub Actions, Docker, AWS ECR, and EC2.

Technologies Used
Python

Machine learning and libraries (Pandas,numpy, Scikit-learn)

MongoDB

FastAPI

Docker

GitHub Actions

AWS (EC2, ECR, S3)

MLflow

