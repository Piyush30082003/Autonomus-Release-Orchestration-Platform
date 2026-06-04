# 🚀 Autonomous Release Orchestration Platform

## 📌 Overview
This project demonstrates a full DevOps CI/CD pipeline that automates build, test, containerization, deployment, and monitoring using modern DevOps tools.

---

## ⚙️ Architecture

GitHub → Jenkins CI → Docker → DockerHub → ArgoCD → Kubernetes → Prometheus → Grafana → Slack Alerts

---

## 🧰 Tech Stack
- Node.js
- Docker
- Kubernetes
- Jenkins
- ArgoCD
- Prometheus
- Grafana
- Helm
- Slack API

---

## 🚀 Features
- CI/CD automation using Jenkins
- Dockerized application deployment
- Kubernetes orchestration
- GitOps using ArgoCD
- Canary deployment using Argo Rollouts
- Monitoring using Prometheus + Grafana
- Auto rollback on failure
- Slack notifications

---

## 📦 How to Run

### Run locally
```bash
node app/app.js
