# Devops_project

🚀 Ultimate CI/CD DevOps Pipeline Project
This repository showcases a complete, production-grade CI/CD pipeline implementation using industry-standard DevOps tools. The project simulates a corporate environment, covering infrastructure setup, secure deployments, and full lifecycle automation of a microservice-based application using Jenkins, Docker, SonarQube, Nexus, Kubernetes, and AWS.

🔧 Tech Stack
Category	Tools & Services
Source Control	GitHub (Private Repo)
CI/CD Orchestration	Jenkins (with scripted pipelines)
Build Tools	Maven, JDK 17
Quality & Security	SonarQube, Trivy, CubeAudit
Artifact Repository	Nexus Repository Manager 3
Containerization	Docker
Container Registry	Docker Hub (private/public)
Orchestration	Kubernetes (multi-node cluster on EC2)
Monitoring	Prometheus (Node Exporter), Grafana, Blackbox Exporter
Hosting/Infra	AWS (EC2, VPC, Security Groups, etc.)

🧩 Project Architecture & Phases
Phase 1: Infrastructure Setup
Created secure VPC & EC2 instances on AWS

Setup Jenkins, SonarQube, Nexus, Docker, and Kubernetes (multi-node)

Configured security groups with proper port access

Cluster scanned with kubeaudit for vulnerabilities

Phase 2: Code Integration
Cloned private GitHub repository and pushed Java-based microservice

Installed & configured Git, GitHub token-based authentication

Phase 3: CI/CD Pipeline Implementation
Jenkins scripted pipeline stages:

🔄 Git Checkout (secured via GitHub PAT)

⚙️ Compilation (mvn compile)

✅ Unit Testing (mvn test)

🔍 Code Quality (SonarQube Scanner)

🛡️ Vulnerability Scans (Trivy - FS + Docker)

📦 Package & Artifact Upload (Nexus via mvn deploy)

🐳 Docker Image Build, Tag, Push

☸️ Kubernetes Deployment

📩 Email Notifications (SMTP via Jenkins)

Phase 4: Monitoring & Observability
Configured:

Blackbox Exporter for endpoint uptime monitoring

Node Exporter + Prometheus + Grafana for system-level insights

📁 Project Structure
bash
Copy
Edit
├── Jenkinsfile              # Complete CI/CD pipeline
├── pom.xml                  # Maven project config
├── Dockerfile               # Docker build config
├── src/                     # Source code
└── scripts/                 # Setup scripts for tools and infrastructure
🛡️ Security Practices
Tokens and credentials managed via Jenkins credential store

Private GitHub repo access via PAT

Docker and Kubernetes images scanned using Trivy and kubeaudit

VPC, IAM, and EC2 hardened using AWS best practices

📌 Prerequisites
AWS account with permissions to manage EC2/VPC

GitHub Personal Access Token

Jenkins admin access

Installed tools: Git, Git Bash, Docker, Jenkins, Java 17, Maven

📬 Notifications & Reporting
Jenkins email notifications enabled via SMTP (port 465)

HTML vulnerability reports exported from Trivy

SonarQube Quality Gate integrated with Jenkins for code acceptance

💡 Key Learnings
Real-world simulation of enterprise DevOps pipeline

End-to-end deployment automation on Kubernetes

Security scanning and best practices in CI/CD environments

Monitoring critical infrastructure using Prometheus stack
