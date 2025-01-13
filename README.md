Lung X-ray Classification with Deep Learning and AWS Deployment

This project focuses on building a robust pipeline for classifying lung X-ray images using deep learning techniques. By leveraging cutting-edge tools and platforms, the project achieves efficient data handling, training, deployment, and monitoring, ensuring high accuracy and performance.

Key Features

Deep Learning with CNN: Implements a Convolutional Neural Network (CNN) for image classification.

Comprehensive Pipeline: Automates data ingestion, transformation, training, evaluation, and deployment.

AWS Integration: Utilizes AWS S3, AWS CLI, and AWS ECR for storage and deployment.

Experiment Tracking: Tracks experiments with MLflow for improved reproducibility.

Data Version Control: Uses DVC for managing and versioning datasets.

CI/CD Automation: Ensures continuous integration and delivery with GitHub Actions and Docker.

Deployment: Deploys the trained model using BentoML.

Technologies Used

Programming and Frameworks:

Python

PyTorch

Scikit-learn

Deployment Tools:

Docker

AWS CLI

BentoML

Version Control and CI/CD:

Git

DVC

GitHub Actions

Experiment Tracking:

MLflow

Pipeline Overview

Data Ingestion:

Collects and stores lung X-ray datasets in AWS S3 for seamless access.

Data Transformation:

Pre-processes the images for training using Python and Scikit-learn.

Model Training:

Trains a CNN model using PyTorch.

Optimizes hyperparameters, including learning rate, for improved performance.

Evaluation:

Achieves significant improvement in accuracy and loss metrics:

Training Accuracy: Increased from 66.19% to 92.38%

Test Accuracy: Achieved 96.67%

Training Loss: Reduced from 0.5766 to 0.0081

Experiment Tracking:

Tracks metrics and parameters using MLflow for reproducibility.

Deployment:

Packages the model with BentoML.

Deploys it to a Docker container hosted on AWS ECR.

CI/CD Integration:

Automates build, test, and deployment pipelines using GitHub Actions and Docker.

Results

Training Accuracy: Improved from 66.19% to 92.38%

Test Accuracy: Reached 96.67%

Training Loss: Reduced from 0.5766 to 0.0081

Optimized Model: Ensured efficient convergence and performance.

How to Run the Project

Prerequisites:

Python (v3.8+)

AWS CLI configured

Docker installed

DVC installed

MLflow configured

Git and GitHub Actions setup

Steps:

Clone the Repository:

git clone [repository_url]
cd [repository_folder]

Set Up Environment:

python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
pip install -r requirements.txt

Configure AWS:

aws configure

Run Data Pipeline:

dvc pull  # To fetch the dataset

Train the Model:

python train.py

Track Experiments:

mlflow ui

Build Docker Image:

docker build -t lung-xray-classification .

Deploy with BentoML:

bentoml serve service:svc

Automate CI/CD:

Push changes to GitHub to trigger the CI/CD pipeline.

Future Enhancements

Integrate advanced model architectures for further accuracy improvements.

Extend the deployment to edge devices for real-time predictions.

Incorporate Explainable AI (XAI) techniques to interpret model predictions.

Contributors

Ujjwal madawat

For any queries, feel free to reach out at ujjwalm9895@gmail.com.

