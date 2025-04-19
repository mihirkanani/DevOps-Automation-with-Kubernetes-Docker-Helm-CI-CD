# 🚀 DevOps Automation with Kubernetes, Docker, Helm, and CI/CD

This project demonstrates a fully automated DevOps workflow using **Kubernetes**, **Docker**, **GitHub Actions**, **Helm**, **ArgoCD**, and **AWS**. It automates the entire build, test, containerization, and deployment pipeline for cloud-native applications.

---

## 📌 Architecture Diagram

![DevOps Automation Architecture](https://github.com/user-attachments/assets/c97bd06d-9ba2-4a88-8982-0065aa9c0a29)

---

## ✅ Project Steps

1. **📥 Clone & Run Locally**
   - Cloned the repository and verified application functionality in local environment.

2. **🐳 Docker Containerization with Distroless**
   - Created a Dockerfile using **distroless** base image to ensure minimal attack surface and size.

3. **☸️ Kubernetes Manifest Creation**
   - Authored YAML files for:
     - `Deployment`
     - `Service`
     - `Ingress`

4. **🌐 Ingress Controller with AWS**
   - Configured **Ingress Controller** (NGINX) to manage external HTTP/S traffic to services.

5. **🌍 DNS Mapping**
   - Mapped Ingress endpoint with **Amazon ELB** for domain-level access to the application.

6. **📦 Helm Chart Creation**
   - Created **Helm charts** with templates for manifests.
   - Managed configurations via `values.yaml`.

7. **🔐 Token-Based Auth**
   - Generated and used **DockerHub** and **GitHub tokens** to authenticate CI/CD pipelines.

8. **⚙️ CI Pipeline via GitHub Actions**
   - Set up automated GitHub Actions pipeline to:
     - Trigger on commit
     - Build and test app
     - Push Docker image to DockerHub
     - Update `values.yaml` with new image version

9. **🚀 CD with ArgoCD**
   - Configured **ArgoCD** to detect changes in the Helm chart repo and redeploy updated containers on **AWS EKS**.

---

## 🎯 Project Outcomes

- ✅ Fully automated CI/CD pipeline using industry-standard tools
- ✅ Production-grade Kubernetes deployment with Helm
- ✅ Distroless Docker containers for secure image builds
- ✅ GitOps-style continuous deployment using ArgoCD
- ✅ Domain access setup via Ingress
- ✅ End-to-end hands-on experience with scalable DevOps systems

---

## 🛠️ Tools & Technologies Used

- **Docker & DockerHub**
- **Kubernetes (EKS on AWS)**
- **Helm**
- **GitHub Actions**
- **ArgoCD**
- **AWS (EKS, ELB)**
- **Distroless Images**
- **NGINX Ingress Controller**

---

