# Sentiment Analysis with MLflow & Prefect (MLOps Project)

This project demonstrates an end-to-end MLOps workflow for a Sentiment Analysis system using MLflow for experiment tracking & model management and Prefect for workflow orchestration and automation.

The goal is to ensure reproducibility, observability, and scalability in a machine learning pipeline.



# Project Objectives
- Track ML experiments using MLflow
- Log parameters, metrics, and artifacts
- Compare multiple models visually
- Register and manage models with tags
- Automate training workflows using Prefect
- Deploy MLflow Tracking Server on AWS
- Containerize the system using Docker



# Use Case
Sentiment analysis of Flipkart-style product reviews, classifying text into:
- Positive
- Neutral
- Negative



# Tech Stack
- Python
- Scikit-learn
- MLflow
- Prefect
- Docker & Docker Compose
- AWS EC2
- TF-IDF + Logistic Regression / Naive Bayes



# Project Structure

mlflow-sentiment-analysis/
│
├── training/
│ └── train_with_mlflow.py
│
├── prefect/
│ └── sentiment_flow.py
│
├── docker/
│ ├── Dockerfile
│ └── docker-compose.yml
│
├── requirements.txt
├── README.md
└── screenshots/
├── mlflow_ui.png
├── model_registry.png
└── prefect_dashboard.png



# MLflow Experiment Tracking
MLflow is used to:
- Log parameters (model type, hyperparameters)
- Log metrics (accuracy, F1-score)
- Store trained models
- Compare multiple runs visually
- Register best-performing models

# Run MLflow UI locally
```bash
mlflow ui

http://localhost:5000

prefect server start

http://127.0.0.1:4200
