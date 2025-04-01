# Spring Boot CI/CD Pipeline with Argo CD & Docker

![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=Jenkins&logoColor=white)
![ArgoCD](https://img.shields.io/badge/Argo%20CD-EF7B4D?style=for-the-badge&logo=Argo&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=Kubernetes&logoColor=white)

A fully automated CI/CD pipeline for deploying Spring Boot applications to Kubernetes using GitOps principles.

## 🚀 Key Features
- **Jenkins CI Pipeline**: Build, test, and package Spring Boot apps with Maven
- **Docker Image Management**: Automated image builds pushed to DockerHub
- **GitOps with Argo CD**: Declarative Kubernetes deployments synced with Git
- **Quality Gates**: Integrated testing (Testify/Scram Qukey) in pipeline
- **Infrastructure as Code**: Kubernetes manifests versioned in Git

## 📦 Prerequisites
- Jenkins server
- Kubernetes cluster
- DockerHub account
- Argo CD installed

## ⚙️ Pipeline Architecture
```plaintext
1. Code Commit → 2. Jenkins (Build → Test → Dockerize) → 3. DockerHub → 4. Argo CD (Sync) → 5. Kubernetes
