# Modular MLOps Pipeline for Phishing Site Classification

An intelligent machine learning-based system to detect and classify phishing websites, helping users and organizations stay protected from online threats.
An end-to-end, production-ready Machine Learning Operations (MLOps) project demonstrating modular design principles, scalable infrastructure, and robust deployment strategies.

---

## 🚀 Project Overview

This project was developed as part of a practical workshop I designed and facilitated, focusing on building **modular MLOps pipelines** for real-world machine learning systems.  
It covers the **entire ML lifecycle** — from **data ingestion**, **feature engineering**, **model training**, to **deployment** — using industry-standard tools such as:

- **Docker** for containerization
- **GitHub Actions** for CI/CD automation
- **AWS EC2** and **ECR** for scalable cloud deployment

The aim is to show how to create **reproducible**, **scalable**, and **production-grade** ML workflows.

---

##  Technologies and Tools Used

- **Python 3.10+**
- **Pandas**, **Scikit-learn** — ML model building and evaluation
- **Docker** — containerized environments
- **GitHub Actions** — continuous integration and continuous delivery (CI/CD)
- **AWS EC2/ECR** — cloud infrastructure deployment
- **Joblib** — model serialization

---

## Pipeline Structure

- **Data Handling**: Modular ETL (Extract, Transform, Load) pipelines
- **Modeling**: Training and evaluation scripts separated cleanly
- **Version Control**: All model artifacts versioned and managed
- **Containerization**: Dockerized application for portability
- **Deployment**: GitHub Actions triggers automatic Docker builds and pushes to AWS ECR, with deployment to EC2
- **CI/CD Best Practices**: Automated testing, linting, building, and deployment

---

## How to Run Locally

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/munal5923/phishing-sites-classifier.git
    cd phishing-sites-classifier
    ```

2. **Set up Virtual Environment and Install Dependencies:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    pip install -r requirements.txt
    ```

3. **Build and Run with Docker (Optional):**

    ```bash
    docker build -t phishing-classifier .
    docker run -p 5000:5000 phishing-classifier
    ```

---

## 🌐 Deployment Workflow

1. **Push Code to GitHub**
2. **GitHub Actions** automatically build the Docker image
3. **Push to AWS ECR**
4. **Deploy the container on AWS EC2 instance**

This ensures **zero downtime deployment**, **automated scaling**, and **full reproducibility** across environments.

---

## Key Highlights

- Full modularization: data processing, model training, inference, and deployment are all separated into clean modules.
- End-to-end automation: From commit to deployment with GitHub Actions workflows.
- Cloud-native deployment: Model served via Docker containers on AWS EC2 instances.
- Focused on production ML system design: reproducibility, automation, scalability, and maintainability.
  
---

## Future Enhancements

- Real-time phishing site detection API
- Improved feature extraction using NLP techniques
- Monitoring and logging (Prometheus, Grafana)
- Full MLOps orchestration (Kubeflow, MLflow integration)

