# DevOpsified CI/CD with Docker, Helm, ArgoCD, and Kubernetes

This repository provides a complete CI/CD pipeline setup using **Docker**, **Helm**, **ArgoCD**, and **Kubernetes**. It demonstrates an automated workflow that integrates continuous integration, continuous deployment, and container orchestration for modern application development.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
  - [Building Docker Image](#building-docker-image)
  - [Deploying with Helm](#deploying-with-helm)
  - [Syncing with ArgoCD](#syncing-with-argocd)
- [Configuration](#configuration)
  - [Docker Configuration](#docker-configuration)
  - [Helm Configuration](#helm-configuration)
  - [ArgoCD Configuration](#argocd-configuration)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

---

## Prerequisites

Before getting started, ensure that you have the following tools installed:

1. **Git**: For cloning the repository.
2. **Docker**: Follow the official [Docker installation guide](https://docs.docker.com/get-docker/) for your operating system.
3. **Helm**: Install Helm by following the instructions [here](https://helm.sh/docs/intro/install/).
4. **Kubernetes**: Use Minikube for a local Kubernetes cluster. Install it by following the guide [here](https://minikube.sigs.k8s.io/docs/).
5. **ArgoCD**: Follow the [ArgoCD installation guide](https://argo-cd.readthedocs.io/en/stable/getting_started/) to deploy it on your Kubernetes cluster.

## Installation

To get started with the project:

1. Clone the repository:
```bash
git clone https://github.com/Rekapost/devopsified-cicd-docker-helm-argocd-k8s.git
cd devopsified-cicd-docker-helm-argocd-k8s
```

2. Install Docker:
Follow the official Docker installation guide.
Verify the installation:
```bash
docker --version
```

3. Install Helm:
Follow the Helm installation guide.

Verify the installation:
```bash
helm version
```

4. Set up Kubernetes:
Use Minikube to create a local Kubernetes cluster. Follow the Minikube installation guide.

Verify the setup:
```bash
kubectl version
```

5. Install ArgoCD:
Follow the ArgoCD installation guide.

Verify the installation:
```bash
argocd version
```

### Usage
#### Building Docker Image
To build the Docker image for your application:
```bash
docker build -t <your_image_name>:<tag> .
```

#### Deploying with Helm
Use Helm to install the application on your Kubernetes cluster:
```bash
helm install <release_name> ./helm
```

#### Syncing with ArgoCD
Once the application is deployed, you can utilize ArgoCD to manage the deployment:

![image](https://github.com/user-attachments/assets/d8da2aeb-e4d0-4095-ba35-16313f47965d)
![image](https://github.com/user-attachments/assets/bf23e294-fc59-4192-93f9-f0c5db560615)
![image](https://github.com/user-attachments/assets/b72fc885-0f1e-426b-8ef4-107ce14b18df)
![image](https://github.com/user-attachments/assets/770695a6-959a-4959-baed-8feba4a66df5)
![image](https://github.com/user-attachments/assets/3b91eab8-1bef-4de6-872f-876c547c3f93)
![image](https://github.com/user-attachments/assets/fb0e7ac9-837d-4c8a-ad8b-c128cff2e163)
![image](https://github.com/user-attachments/assets/7aa2a25b-6f4e-41ba-95ad-b4323589df17)
![image](https://github.com/user-attachments/assets/69bc3835-426c-4f11-9a5f-9e91df126580)
![image](https://github.com/user-attachments/assets/04cff97c-8fbb-4e88-9aee-089b90f2e389)
![image](https://github.com/user-attachments/assets/9ab03b42-8e46-4442-9ded-119f37361598)
![image](https://github.com/user-attachments/assets/c39e6181-89a0-490a-8c56-05f45fbb100b)
![image](https://github.com/user-attachments/assets/3377e853-6d43-4664-b762-f6e49d0751f8)
![image](https://github.com/user-attachments/assets/89063be4-5b51-4c13-9f14-df9ccbb18f6f)
![image](https://github.com/user-attachments/assets/80d295a0-2c1c-4233-817c-c22aafe11fb6)
![image](https://github.com/user-attachments/assets/7354ae87-00c7-429d-ac2e-3e0b68466e95)
![image](https://github.com/user-attachments/assets/62a6869f-281c-4eef-8a40-1907a8540b7b)  
