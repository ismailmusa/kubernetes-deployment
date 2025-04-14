# 📦 Kubernetes Deployment for MongoDB and Mongo Express

This project demonstrates how to deploy a MongoDB database together with Mongo Express—a web-based MongoDB admin interface—within a Kubernetes cluster. It includes a collection of YAML configuration files to simplify deployment, configuration, and service exposure.

## 🔧 What's Included

- **`mongodb-deployment.yml`**: Defines the deployment and service for the MongoDB database.
- **`mongo-express-deployment.yml`**: Sets up the Mongo Express interface, allowing users to interact with MongoDB through a web UI.
- **`configmap.yml`**: Contains configuration data that can be injected into the Mongo Express deployment.
- **`secret.yml`**: Stores sensitive information, such as MongoDB credentials, securely.
- **`ingress.yml`**: Configures ingress resources to manage external access to the Mongo Express service.

## 🚀 Features

- **Declarative Configuration**: Utilizes YAML manifests to define the desired state of the applications.
- **Separation of Concerns**: Employs ConfigMaps and Secrets to manage configuration and sensitive data independently.
- **Web-Based Interface**: Provides Mongo Express for easy interaction with the MongoDB database.
- **Ingress Setup**: Facilitates external access to Mongo Express through Kubernetes Ingress resources.

## 🛠️ Prerequisites

- A running Kubernetes cluster (e.g., Minikube, Kind, or a cloud-based Kubernetes service).
- `kubectl` command-line tool installed and configured to interact with your cluster.

## ▶️ Getting Started

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ismailmusa/kubernetes-deployment.git
   
   cd kubernetes-deployment
   
Apply the Kubernetes Configurations: Run the following commands to deploy MongoDB, Mongo Express, and supporting resources:

kubectl apply -f secret.yml

kubectl apply -f configmap.yml

kubectl apply -f mongodb-deployment.yml

kubectl apply -f mongo-express-deployment.yml

kubectl apply -f ingress.yml

Verify the Deployments: Ensure that the pods, services, and ingress resources are running correctly:

kubectl get pods

kubectl get services

kubectl get ingress


