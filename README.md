## 🚀 CI/CD Corporate Automation Pipeline Using DevOps in AWS

![CI/CD](https://img.shields.io/badge/Automation-CI%2FCD-blue?style=flat-square)
![DevOps](https://img.shields.io/badge/DevOps-AWS%20%7C%20Jenkins%20%7C%20Kubernetes-critical?style=flat-square)

> This project delivers a secure, scalable, and intelligent **CI/CD pipeline** using industry-leading DevOps tools hosted in **Amazon Web Services (AWS)**. Designed for corporate environments, it incorporates security, real-time monitoring, container orchestration, and seamless automation of deployments.

---

### 📽️ Demo Video

[![Watch the video](https://img.youtube.com/vi/M-I6-562JDI/0.jpg)](https://www.youtube.com/watch?v=M-I6-562JDI)

---

### 🎯 Project Objectives

* Automate the software delivery lifecycle (build → test → deploy → monitor)
* Ensure **secure, tested, and compliant** deployments
* Minimize human error and manual overhead
* Enable **real-time observability** with performance metrics and alerts

---

### 🏗️ Architecture Overview

![Architecture Diagram](https://github.com/Jsujanchowdary/CI-CD-Corporate-Automation-Pipeline/blob/main/pipeline%20arc.png)
*Includes Jenkins, Docker, Kubernetes, SonarQube, Nexus, Prometheus, Grafana in AWS.*

---

### 🧩 Modules & Tools Breakdown

| Module                      | Tool/Service         | Description & Benefits                                                                                                            |
| --------------------------- | -------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **CI Orchestration**        | Jenkins              | Manages the end-to-end CI/CD pipeline. Triggers builds on code push, integrates with Docker, Kubernetes, SonarQube, etc.          |
| **Containerization**        | Docker               | Packages applications with all dependencies into lightweight containers. Ensures portability and consistency across environments. |
| **Container Orchestration** | Kubernetes           | Handles scaling, load balancing, self-healing, and rolling deployments of Dockerized applications.                                |
| **Code Quality**            | SonarQube            | Automates code review. Detects bugs, security hotspots, and code smells to maintain high coding standards.                        |
| **Artifact Management**     | Nexus Repository     | Secure storage of build artifacts (e.g., JARs, Docker images) with version control.                                               |
| **Security Analysis**       | Trivy                | Scans Docker images and filesystems for vulnerabilities and misconfigurations before deployment.                                  |
| **Monitoring & Alerts**     | Prometheus + Grafana | Collects, analyzes, and visualizes real-time metrics (CPU, memory, HTTP traffic, probe durations). Enables proactive maintenance. |
| **Infrastructure Hosting**  | AWS (EC2, VPC, S3)   | Provides scalable, cloud-based compute and networking for all pipeline components.                                                |
| **Version Control**         | GitHub/GitLab        | Stores codebase and Jenkins pipeline scripts with access controls.                                                                |
| **Notification System**     | Jenkins Email Ext    | Sends build success/failure, test alerts, and security scan notifications to stakeholders.                                        |

---

### ⚙️ CI/CD Pipeline Workflow

1. **Code Commit** → Source Code pushed to GitHub
2. **Build Stage** → Jenkins compiles with Maven
3. **Unit Testing** → Jenkins runs unit/integration tests
4. **Static Analysis** → SonarQube checks for bugs, security flaws
5. **Image Creation** → Docker builds container image
6. **Image Scan** → Trivy scans the image for vulnerabilities
7. **Artifact Push** → Artifact pushed to Nexus
8. **Deploy** → Kubernetes deploys app across cluster nodes
9. **Monitoring** → Prometheus + Grafana track app & infrastructure
10. **Alerts/Emails** → Stakeholders receive real-time notifications

---

### 📂 Directory Structure

```
.
├── Jenkinsfile                  # CI/CD pipeline definition
├── deploy/                     # Kubernetes manifests (YAML)
├── docker/                     # Dockerfiles and Trivy config
├── scripts/                    # Automation scripts for AWS, Jenkins setup
├── dashboards/                 # Grafana JSON templates
├── sonarqube-config/           # SonarQube project settings
├── README.md                   # This documentation
```

---

### ✅ Key Features

* 🔁 **Fully Automated CI/CD Lifecycle**
* 🛡️ **Integrated Security (Trivy + RBAC + HTTPS)**
* 📈 **Proactive Monitoring with Grafana Dashboards**
* 🚀 **Multi-node Kubernetes Cluster for Scalability**
* 📦 **Nexus for Secure Artifact Storage**
* 📬 **Jenkins Email Notifications for All Stakeholders**

---

### 🔐 Security Highlights

* Role-Based Access Control (RBAC) on Jenkins & Kubernetes
* Docker image scanning before deployment
* Code quality gate to block low-quality code pushes
* HTTPS (TLS) recommended for all dashboards & endpoints

---

### 📊 Sample Dashboard

![Grafana Dashboard](https://github.com/Jsujanchowdary/CI-CD-Corporate-Automation-Pipeline/blob/main/dashboard.png)

---

### 📚 References

* Trivy: [https://github.com/aquasecurity/trivy](https://github.com/aquasecurity/trivy)
* Jenkins Docs: [https://www.jenkins.io/doc/](https://www.jenkins.io/doc/)
* SonarQube: [https://www.sonarqube.org/](https://www.sonarqube.org/)
* Prometheus: [https://prometheus.io/](https://prometheus.io/)
* Grafana: [https://grafana.com/](https://grafana.com/)
* Kubernetes: [https://kubernetes.io/](https://kubernetes.io/)

---

### 👨‍💻 Contributors

* Jujjavarapu Sujan Chowdary
* Naga Venkata Sivanikhil Maradani

Guided by **Prof. Annapurani Panaiyappan**, SRM Institute of Science and Technology

