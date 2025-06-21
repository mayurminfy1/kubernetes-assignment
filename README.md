# 🚀 MongoDB + Mongo Express Deployment on Kubernetes

A complete setup of a MongoDB database and a Mongo Express web UI deployed on a Minikube cluster using Kubernetes best practices like `Secrets`, `ConfigMaps`, `Deployments`, and `Services`.

---

### 📋 Overview

| Section         | Details |
|----------------|---------|
| 🎯 **Objective** | Deploy a full-stack web app using Kubernetes on Minikube — MongoDB backend with a Mongo Express frontend. |
| 🧠 **Background** | This project simulates a real-world web application architecture using Kubernetes components: Pods, Services, Secrets, and ConfigMaps. |
| 🔧 **Prerequisites** | 	<ul><li>✅ Minikube installed and running</li><li>✅ kubectl configured</li><li>✅ VS Code or any text editor</li></ul>|

---

### 🛠️ Kubernetes Commands

| Command | What It Does |
|--------|---------------|
| `kubectl apply -f <file>.yaml` | Create Kubernetes resources |
| `kubectl get all` | View status of pods, services, deployments |
| `kubectl delete -f <file>.yaml` | Delete resources |
| `minikube service mongo-express-service` | Launch the Mongo Express UI in browser |

---

## 📁 Folder Structure

![Folder structure](https://github.com/mayurminfy1/photos/blob/main/kubernetes-takehome/Screenshot%202025-06-21%20160025.png?raw=true)

### 📸 Screenshots

| Description                   | Preview |
|-------------------------------|---------|
| ✅ Starting Minikube     | ![Starting Minikube](https://github.com/mayurminfy1/photos/blob/main/kubernetes-takehome/Screenshot%202025-06-21%20160104.png?raw=true) |
| 🔗 All pods working| ![All pods](https://github.com/mayurminfy1/photos/blob/main/kubernetes-takehome/Screenshot%202025-06-21%20155933.png?raw=true) |
| 🌍 Mongo-Express-Service     | ![Service](https://github.com/mayurminfy1/photos/blob/main/kubernetes-takehome/Screenshot%202025-06-21%20160002.png?raw=true) |
| 🗑 Mongo Express         | ![Mongo Express](https://github.com/mayurminfy1/photos/blob/main/kubernetes-takehome/Screenshot%202025-06-21%20155749.png?raw=true) |
| 🗑 CleanUp         | ![Cleanup](https://github.com/mayurminfy1/photos/blob/main/kubernetes-takehome/Screenshot%202025-06-21%20160233.png?raw=true) |


---

### Creating Secret

```
# PowerShell base64 encoding:
[Convert]::ToBase64String([System.Text.Encoding]::UTF8.GetBytes("my-admin-user"))
# Output: bXktYWRtaW4tdXNlcg==

[Convert]::ToBase64String([System.Text.Encoding]::UTF8.GetBytes("my-super-secret-password"))
# Output: bXktc3VwZXItc2VjcmV0LXBhc3N3b3Jk
```
---

## 🔗Summary

✅ This project demonstrates container orchestration using Kubernetes:

🔐 Secure secrets with Secret

🧩 Environment management with ConfigMap

🌐 Expose services via LoadBalancer

🧱 Real-world separation of backend and frontend via Services Summary

---
