## 📌 Phase 3: CI/CD Pipeline Implementation (Automated Workflows)

Here we built a **fully automated Jenkins pipeline** that replicates enterprise-grade DevOps workflows:

### 🛠 Continuous Integration (CI):
- Automatically pulls code from GitHub
- Compiles Java code using **Maven**
- Runs **unit tests** to catch early bugs
- Performs **code quality scans** with SonarQube (bugs, vulnerabilities, code smells)
- Executes **Trivy file system scan** to detect secrets or vulnerable dependencies in the repo

### 🚀 Continuous Deployment (CD):
- Packages the application and uploads artifacts to **Nexus**
- Builds, tags, and pushes Docker images to **Docker Hub**
- Deploys the Dockerized app to **Kubernetes** with rollout strategy
- Sends **email notifications** on pipeline success or failure

🎯 *Goal*: Automate the entire build → test → scan → deploy pipeline with minimal manual intervention, while following security best practices.
