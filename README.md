# 📦 Kubernetes Deployment

This repository provides a simple and practical example of deploying a containerized application to a Kubernetes cluster using deployment and service YAML configurations.

- `deployment.yaml`: Defines the desired state of the application, including the container image, number of replicas, and pod specifications.
- `service.yaml`: Exposes the deployed pods via a Kubernetes Service, enabling network access to the application.

## 🚀 Features

- Declarative Kubernetes deployment using YAML manifests.
- Scalable application architecture with replicas.
- Basic service exposure for internal or external access (ClusterIP/NodePort/LoadBalancer).
- Ready-to-use example to get started with Kubernetes deployments.

## 🛠️ Prerequisites

- A running Kubernetes cluster (Minikube, Kind, or any cloud provider).
- `kubectl` installed and configured to access your cluster.

## ▶️ Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/ismailmusa/kubernetes-deployment.git
   cd kubernetes-deployment
   
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl get pods
kubectl get services


