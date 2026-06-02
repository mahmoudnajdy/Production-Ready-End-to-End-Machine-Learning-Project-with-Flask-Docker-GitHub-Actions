# 🏠 End-to-End House Price Prediction System

A production-style Machine Learning application that predicts house prices through a web interface and demonstrates the complete ML Engineering lifecycle—from model development to cloud deployment.

## 🚀 Live Demo

**Application URL:**
`http://98.91.240.38:5000`

> Deployed on AWS EC2 using Docker and automated CI/CD with GitHub Actions.

---

## 📌 Project Overview

This project demonstrates how to take a Machine Learning model from a local development environment and deploy it as a cloud-hosted application accessible through a web browser.

The project covers:

* Data preprocessing and feature engineering
* Model training and evaluation
* Model serialization
* Flask web application development
* Docker containerization
* CI/CD automation using GitHub Actions
* Cloud deployment on AWS EC2

---

## 🏗️ System Architecture

```text
User
 │
 ▼
Flask Web Application
 │
 ▼
Preprocessing Pipeline
 │
 ▼
Machine Learning Model
 │
 ▼
Prediction Result
```

### Deployment Architecture

```text
Developer
    │
    ▼
GitHub Repository
    │
    ▼
GitHub Actions
    │
    ▼
Docker Hub
    │
    ▼
AWS EC2
    │
    ▼
Running Docker Container
```

---

## ⚙️ Tech Stack

### Machine Learning

* Python
* Scikit-Learn
* NumPy
* Pandas

### Visualization

* Matplotlib
* Seaborn

### Backend

* Flask
* Gunicorn

### DevOps & Deployment

* Docker
* GitHub Actions
* Docker Hub
* AWS EC2
* SSH

---

## 🔄 CI/CD Pipeline

Every push to the `main` branch automatically:

1. Builds a new Docker image
2. Pushes the image to Docker Hub
3. Connects to AWS EC2 via SSH
4. Stops the currently running container
5. Pulls the latest image
6. Starts the new version

This ensures fully automated deployments without manual intervention.

---

## 📂 Project Structure

```text
.
├── .github/workflows/
│   └── deploy.yml
├── templates/
│   └── home.html
├── app.py
├── model.pkl
├── scaler.pkl
├── requirements.txt
├── Dockerfile
└── README.md
```

---

## 🐳 Docker

Build image:

```bash
docker build -t house-price-app .
```

Run container:

```bash
docker run -d -p 5000:5000 house-price-app
```

---

## ☁️ AWS Deployment

The application is deployed on:

* AWS EC2
* Ubuntu Server
* Docker Container
* GitHub Actions CI/CD

The deployment pipeline automatically updates the running application whenever new code is pushed.

---

## 🎯 Key Engineering Challenges Solved

During development and deployment I worked through several real-world engineering challenges:

* Docker image creation and optimization
* Dependency management
* GitHub Actions workflow configuration
* Docker Hub integration
* SSH authentication and key management
* EC2 server configuration
* Docker permissions on Linux
* AWS Security Group configuration
* Automated container replacement during deployment

---

## 🔮 Future Improvements

* FastAPI migration
* Pytest unit testing
* Model monitoring
* Infrastructure as Code (Terraform)
* Nginx reverse proxy
* HTTPS with Let's Encrypt
* AWS ECS deployment
* Kubernetes orchestration

---

## 👨‍💻 Author

Mahmoud

Mechatronics Engineer transitioning into AI & Machine Learning Engineering.

Currently focused on:

* Machine Learning Engineering
* MLOps
* Cloud Deployment
* Computer Vision
* Production AI Systems

```
```
