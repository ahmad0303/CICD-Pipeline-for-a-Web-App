# 🚀 Full-Stack CI/CD Pipeline with Docker, GitHub Actions & Kubernetes

This project demonstrates a complete **CI/CD pipeline** setup for a containerized full-stack web application using **GitHub Actions**, **Docker**, and **Kubernetes**. The app is based on a test project using **React** (client) and **Node.js/Express** (API).

---

## 🧱 Tech Stack

- **Frontend**: React
- **Backend**: Node.js
- **CI/CD**: GitHub Actions
- **Containerization**: Docker
- **Orchestration**: Kubernetes with Helm Chart
- **Deployment Target**: Any K8s cluster (Minikube)
- **Registry**: Docker Hub (configurable)

---

## ⚙️ Features

- ✅ Dockerized both frontend and backend apps
- ✅ Automated CI/CD with GitHub Actions
- ✅ Builds and pushes Docker images to Docker Hub
- ✅ Deploys to Kubernetes cluster
- ✅ Easily extendable with Helm Chart

---

## Quick Start
```
# Clone the repository
git clone https://github.com/ahmad0303/CICD-Pipeline-for-a-Web-App.git

# Go inside the directory
cd CICD-Pipeline-for-a-Web-App

# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm start
```
---

## Local Docker Test
```
docker build -t cicd-project-reactapp-image .
docker run -p 8080:8080 cicd-project-reactapp-image
```

---

## 🚀 Deploy with Helm

1. Install Chart:
```helm install cicdproj-chart ./cicdproj-chart```

2. Upgrade Deployment:
```helm upgrade cicdproj-chart ./cicdproj-chart```

3. Uninstall:
```helm uninstall cicdproj-chart```

---

## 🔐 GitHub Actions CI/CD
You can automate the build & deployment process using a .github/workflows/deploy.yml file.

Set GitHub Secrets:
- DOCKER_USERNAME
- DOCKER_PASSWORD

### Workflow Steps:
Checkout code
Build Docker image
Push to DockerHub
Deploy to K8s using Helm

---

## Leave a ⭐ on the repo if you found this helpful!