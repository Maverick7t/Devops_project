## 📌 Phase 1: Infrastructure Setup (AWS-based)

In this phase, we lay the foundation by provisioning secure, scalable infrastructure on AWS:

- Created a **Virtual Private Cloud (VPC)** to isolate all components and restrict public exposure
- Launched EC2 instances to serve different roles: 
  - Jenkins (CI server)
  - SonarQube (code quality analysis)
  - Nexus (artifact repository)
  - Kubernetes (1 master, 2 workers)
- Configured **Security Groups (firewall rules)** to allow only essential ports (e.g. 22, 80, 443, 8080, 9000)
- Installed critical software (Java 17, Docker, Git, Jenkins, etc.)
- Deployed and validated a **Kubernetes cluster** from scratch
- Performed a security scan using `kubeaudit` to identify misconfigurations

🎯 *Goal*: Establish a secure, isolated environment to run the DevOps pipeline in a cloud-native manner.




