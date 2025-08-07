# 🚀 Ultimate CI/CD DevOps Pipeline Project

This repository demonstrates a full-scale **CI/CD DevOps pipeline** implementation tailored for real-world enterprise environments. Built from scratch, the pipeline integrates infrastructure provisioning, secure deployments, quality assurance, and monitoring using the modern DevOps toolchain.

---

## 🔧 Tech Stack

| Category            | Tools & Services                             |
|---------------------|----------------------------------------------|
| Source Control      | GitHub (Private Repository)                  |
| CI/CD Orchestration | Jenkins (Scripted Pipelines)                 |
| Build Tools         | Maven, JDK 17                                |
| Quality & Security  | SonarQube, Trivy, kubeaudit                  |
| Artifact Repository | Nexus Repository Manager 3                   |
| Containerization    | Docker                                       |
| Container Registry  | Docker Hub                                   |
| Orchestration       | Kubernetes (Multi-node on AWS EC2)           |
| Monitoring          | Prometheus, Grafana, Node Exporter, Blackbox Exporter |
| Infrastructure      | AWS (EC2, VPC, Security Groups)              |

---

## 🧩 Project Architecture

![Pipeline Monitoring](https://github.com/Maverick7t/Devops_project/blob/main/Phase_1/Screenshot%202025-08-07%20105126.png)

## 🧩 Project Phases

### Phase 1: Infrastructure Setup
- Provisioned VPC, Security Groups, and EC2 instances
- Configured Jenkins, SonarQube, Nexus, and Docker
- Set up a secure Kubernetes cluster (1 Master + 2 Worker Nodes)
- Performed cluster security audit using `kubeaudit`

### Phase 2: Source Code Integration
- Created a **private GitHub repo**
- Pushed Java-based microservice using Git + Git Bash
- Token-based GitHub authentication via Jenkins credentials

### Phase 3: CI/CD Pipeline in Jenkins
Pipeline stages include:
- 🔄 **Git Checkout**
- ⚙️ **Code Compilation**: `mvn compile`
- ✅ **Unit Testing**: `mvn test`
- 🧹 **SonarQube Code Quality Check**
- 🛡️ **Trivy FS Scan**: Detect secrets & vulnerable dependencies
- 📦 **Package & Artifact Upload** to Nexus via `mvn deploy`
- 🐳 **Docker Image Build, Tag, and Push** to Docker Hub
- ☸️ **Kubernetes Deployment** of the app
- 📧 **Email Notifications** for pipeline success/failure

### Phase 4: Monitoring
- 🔍 **System Monitoring** using Node Exporter + Prometheus + Grafana
- 🌐 **Website Uptime Monitoring** via Blackbox Exporter

---



