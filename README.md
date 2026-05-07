# 🚀 End-to-End NLP Text Summarization Pipeline

## 📌 Project Overview
This project is an end-to-end Natural Language Processing (NLP) Text Summarization system built using a modular MLOps pipeline approach. It includes data ingestion, validation, transformation, model training, evaluation, and deployment using Flask, Docker, AWS, and GitHub Actions CI/CD. This implementation is based on a reference architecture and was executed and extended by me for hands-on learning of NLP pipelines, MLOps workflows, and production deployment.

## ⚙️ Project Workflow
1. Update config.yaml  
2. Update params.yaml  
3. Define entity classes  
4. Build Configuration Manager in src/config  
5. Develop pipeline components (data ingestion, validation, transformation, model training, evaluation)  
6. Create training pipeline  
7. Update main.py  
8. Integrate app.py  

## 🧠 Tech Stack
Python 3.8, NLP (Text Summarization), Flask, PyTorch/Transformers, Docker, AWS (EC2 & ECR), GitHub Actions, Git & GitHub

## 🚀 How to Run This Project
### Step 1: Clone Repository
git clone https://github.com/krishnaik06/Text-Summarization-NLP-Project.git  
cd Text-Summarization-NLP-Project  

### Step 2: Create Environment
conda create -n summary python=3.8 -y  
conda activate summary  

### Step 3: Install Dependencies
pip install -r requirements.txt  

### Step 4: Run Application
python app.py  

Open browser: http://localhost:5000  

## ☁️ AWS CI/CD Deployment
This project uses Docker + AWS ECR + EC2 + GitHub Actions for CI/CD automation.

### IAM Setup
Create IAM user with EC2 and ECR access and attach:
- AmazonEC2ContainerRegistryFullAccess  
- AmazonEC2FullAccess  

### ECR Setup
Create repository and store image:
aws_account_id.dkr.ecr.region.amazonaws.com/text-summarizer  

### EC2 Setup
sudo apt-get update -y  
sudo apt-get upgrade -y  
curl -fsSL https://get.docker.com -o get-docker.sh  
sudo sh get-docker.sh  
sudo usermod -aG docker ubuntu  
newgrp docker  

### GitHub Runner Setup
Go to GitHub → Settings → Actions → Runners → New Self Hosted Runner and follow commands.

### GitHub Secrets
AWS_ACCESS_KEY_ID  
AWS_SECRET_ACCESS_KEY  
AWS_REGION  
AWS_ECR_LOGIN_URI  
ECR_REPOSITORY_NAME  

## 📊 Features
End-to-end NLP pipeline, modular code structure, Flask web app, Docker containerization, AWS deployment, CI/CD automation

## 👨‍💻 Author
Prajwal H – Aspiring Data Scientist / ML Engineer

## 🎯 Learning Outcome
Learned real-world NLP pipeline design, MLOps architecture, CI/CD automation, Docker, AWS deployment, and modular ML system development.

## ⭐ Note
This project is implemented for learning and understanding industry-level MLOps and NLP pipeline architecture based on a reference project, with personal execution and enhancements.
