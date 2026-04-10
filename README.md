# Kubernetes Scalable App 🚀

## Features
- Node.js app containerized with Docker
- Deployed on Kubernetes
- Load balanced using Service
- Auto scaling using HPA

## Run Steps

### 1. Build Docker Image
docker build -t devmahalle/k8s-app .

### 2. Push to Docker Hub
docker push devmahalle/k8s-app

### 3. Start Kubernetes
minikube start

### 4. Deploy
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f hpa.yaml

### 5. Access App
minikube service k8s-service

## Commands
kubectl get pods
kubectl get svc
kubectl get hpa
