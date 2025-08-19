# GitOps Platform Automation

> Automating Kubernetes application deployment using GitOps principles with Terraform and ArgoCD.

## 🧠 Problem Solved
Manual deployment to Kubernetes is error-prone and hard to scale. GitOps solves this by automating everything through version-controlled, declarative manifests.

## 🔧 Tools Used
- Terraform
- ArgoCD
- Kubernetes (GKE)
- Docker
- GitHub Actions

## ⚙️ Architecture
(Loading...)

## 🚀 Setup Instructions
1. Provision GKE using Terraform
2. Install ArgoCD
3. Configure ApplicationSet
4. Push sample app and let ArgoCD auto-sync it

## 📸 Demo
(Coming soon)

## Quick Start

# 1) Install Argo CD
kubectl create ns argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

# 2) Create the Argo CD Application (after updating repoURL in yaml)
kubectl apply -n argocd -f argo-apps/nginx-app.yaml

# 3) Watch it sync
kubectl get applications -n argocd

# 4) Get the app endpoint
kubectl get svc nginx -n default


## 🧠 Lessons Learned
(coming up)

---
