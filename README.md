# 🎮 2048 Game on Amazon EKS with ALB Ingress

This repository contains all necessary files to deploy the **2048 web game** on an **Amazon EKS cluster**, exposed publicly using the **AWS ALB Ingress Controller**.

---

## 📌 Overview

- ✅ Deploys a containerized 2048 game
- 🚀 Uses **Amazon EKS** for managed Kubernetes
- 🌐 Application is exposed using **AWS ALB Ingress Controller**
- 🔐 IAM is configured with **IRSA** (IAM Role for Service Account)

---

## 🧰 Prerequisites

- AWS CLI (`aws configure`)
- `kubectl`
- `eksctl`
- `helm`
---

## 🔧 EKS Cluster Setup

Create the cluster using `eksctl`:

```bash
eksctl create cluster \
  --name maddy-cluster \
  --region ap-south-1 \
