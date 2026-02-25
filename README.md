## End-to-End Text Summarization using NLP & Transformers

An end-to-end abstractive text summarization system built using Transformer-based models (PEGASUS).
This project demonstrates a complete production-grade ML workflow including modular pipeline design, Docker containerization, CI/CD automation, and AWS deployment.

Focus: Not just model training — but building a deployable, scalable ML system.



### 🚀 Project Overview

This project implements a full machine learning pipeline that:

Ingests and preprocesses text data

Fine-tunes a Transformer model for summarization

Evaluates model performance

Exposes predictions via a FastAPI REST API

Containerizes the application using Docker

Automates CI/CD using GitHub Actions

Deploys on AWS EC2 using Amazon ECR




### 🧠 Model Architecture
PEGASUS (Encoder–Decoder Transformer)

Built using Hugging Face Transformers

Designed for abstractive text summarization

Trained using cross-entropy loss for next-token prediction

Encoder–Decoder Intuition

Encoder → Converts input text into contextual embeddings

Decoder → Generates summary based on encoded meaning

The model learns to generate shorter, meaningful summaries while preserving context




### 🏗️ Project Structure

Text-Summarization-using-NLP/
│
├── src/textSummarizer/
│   ├── components/         # Data ingestion & model components
│   ├── pipeline/           # Training & prediction pipelines
│   ├── config/             # Configuration management
│   ├── utils/              # Utility functions
│
├── artifacts/              # Model artifacts (ignored in Git)
├── app.py                  # FastAPI application
├── Dockerfile              # Docker configuration
├── requirements.txt
├── .github/workflows/      # CI/CD pipeline
└── README.md




### ⚙️ Features

✔ Modular ML pipeline
✔ Configuration-driven design
✔ Transformer-based summarization
✔ FastAPI inference endpoint
✔ Dockerized deployment
✔ GitHub Actions CI/CD
✔ AWS ECR integration
✔ EC2 self-hosted deployment




### 🔁 CI/CD Workflow
Continuous Integration

Triggered on push to main:

Checkout code

Lint checks

Unit tests

Continuous Delivery

Build Docker image

Tag and push image to Amazon ECR

Continuous Deployment

Self-hosted GitHub runner on EC2

Pull latest image

Run container on port 8080

Cleanup old images




### 🐳 Docker Usage
Build Image
docker build -t text-summarizer .

Run Container
docker run -p 8080:8080 text-summarizer


Access API at:

http://localhost:8080

☁️ AWS Deployment

The project uses:

Amazon ECR → Container registry

Amazon EC2 → Hosting environment

GitHub Self-Hosted Runner → Automated deployment

IAM Credentials → Secure AWS authentication

Deployment is fully automated through GitHub Actions.




### 📊 Tech Stack

Python

Hugging Face Transformers

PyTorch

FastAPI

Docker

GitHub Actions

AWS (ECR, EC2)

YAML-based configuration



### 🧪 Run Locally
git clone https://github.com/sanskar1dethe/Text-Summarization-using-NLP.git
cd Text-Summarization-using-NLP
pip install -r requirements.txt
python app.py




### 📈 Key Learnings

Transformer Encoder–Decoder architecture

Building modular ML pipelines

Docker optimization and debugging

CI/CD automation

AWS container deployment

Managing ML dependencies in production

👤 Author

Sanskar Dethe
B.Tech Mathematics & Computing | IIT Goa
AI Engineer | NLP | MLOps | Production ML Systems



# END TO END Text-Summarization-using-NLP

# Workflow 

1. Update config.yaml 
2. Update params.yaml
3. Update entities.yaml
4. Update the configuration manager in src config
5. Update the components
6. Update the pipeline 
7. Update main.py
8. Update app.py

