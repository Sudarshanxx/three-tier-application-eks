🚀 Three-Tier To-Do List Application Deployment on AWS EKS
📌 Overview

This repository contains my end-to-end Three-Tier Web Application project, where I designed, containerized, and deployed a To-Do List application using modern cloud-native and DevOps tools.

The project demonstrates real-world DevOps practices, including Dockerization, Kubernetes orchestration, AWS EKS deployment, Infrastructure as Code (Terraform), and CI/CD planning with Jenkins.

🧩 Application Architecture (Three-Tier)

Frontend

ReactJS (To-Do List UI)

Backend

NodeJS + Express

REST APIs for task management

Database

MongoDB

Persistent storage using Kubernetes PVCs

Deployment Platform

AWS EKS (Elastic Kubernetes Service)

🛠️ Tech Stack Used
Cloud & Infrastructure

AWS (EKS, EC2, IAM, ECR, VPC)

Terraform (Infrastructure as Code)

Containers & Orchestration

Docker

Kubernetes (Deployments, Services, PVC, ConfigMaps, Secrets)

CI/CD & DevOps

Jenkins (Pipeline planning)

GitHub (Version Control)

Planned GitOps & CI/CD automation

Monitoring & Future Enhancements

Helm

Prometheus & Grafana (planned)

ArgoCD (planned)

📂 Project Structure
TWSThreeTierAppChallenge/
├── Application-Code/
│   ├── frontend/        # React To-Do application
│   └── backend/         # NodeJS API with MongoDB
├── Kubernetes-Manifests-file/
│   ├── frontend/
│   ├── backend/
│   └── database/
├── Jenkins-Pipeline-Code/
│   └── README.md        # Planned CI/CD pipeline
├── Jenkins-Server-TF/
│   ├── vpc.tf
│   ├── ec2.tf
│   ├── iam-role.tf
│   └── backend.tf
├── assets/              # Screenshots & diagrams
└── README.md

📦 Application Code
Frontend (React – To-Do List)

Task creation, update, and deletion

API integration with backend service

Containerized using Docker

Backend (NodeJS + Express)

REST APIs

MongoDB connection

Secure credentials using Kubernetes Secrets

Dockerized for EKS deployment

☸️ Kubernetes Deployment (AWS EKS)

Namespace-based deployment

Backend & frontend services

MongoDB with PersistentVolumeClaim

Private Amazon ECR images

LoadBalancer service for external access

🏗️ Jenkins Server Infrastructure (Terraform)

The Jenkins-Server-TF directory contains Terraform code to provision:

Custom VPC

EC2 instance for Jenkins

IAM roles & instance profiles

Security groups

Automated tool installation

⚠️ Status: Infrastructure code prepared.
Jenkins pipeline execution is planned as a future enhancement.

🔁 Jenkins Pipeline (Planned)

The Jenkins-Pipeline-Code directory contains:

Planned CI/CD workflow

Automated Docker build

Push images to Amazon ECR

Deploy updates to AWS EKS

Included to demonstrate CI/CD design knowledge and future extensibility.

🧪 Key Challenges Solved

Debugged ImagePullBackOff & IAM permission issues

Resolved CrashLoopBackOff due to container entrypoint problems

Implemented Persistent Volumes for MongoDB

Managed ECR authentication with EKS Node IAM roles

Designed clean Kubernetes manifests for production-style deployment

🚀 How to Run (High-Level)

Provision EKS cluster using eksctl

Build & push Docker images to Amazon ECR

Apply Kubernetes manifests

Verify pods, services, and load balancer

Access the To-Do application via external endpoint

🧹 Cleanup
eksctl delete cluster --name three-tier-cluster --region us-west-2


Also delete:

EC2 instances

Load Balancers

Security groups
to avoid AWS charges.

🎯 What I Learned

Real-world AWS EKS deployment workflows

Kubernetes debugging at production level

IAM best practices for ECR & EKS

Infrastructure as Code using Terraform

CI/CD architecture design with Jenkins

📌 Project Status

✅ Fully deployed Three-Tier To-Do List Application
🛠️ CI/CD automation & monitoring planned

🤝 Contribution

This project is part of my learning and portfolio development.
Suggestions and improvements are welcome via issues or pull requests.

🌟 Connect

If you’re interested in DevOps, Cloud, or Kubernetes projects, feel free to connect with me on LinkedIn or explore this repository.

Happy Building & Learning 🚀
