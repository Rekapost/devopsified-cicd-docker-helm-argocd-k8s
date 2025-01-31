# DevOpsified CI/CD with Docker, Helm, ArgoCD, and Kubernetes

This project demonstrates a complete CI/CD pipeline setup using **Docker**, **Helm**, **ArgoCD**, and **Kubernetes**. It provides an end-to-end automated deployment flow that integrates continuous integration, continuous deployment, and container orchestration for modern application development.

## Table of Contents

- [Introduction](#introduction)
- [Architecture](#architecture)
- [Prerequisites](#prerequisites)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project serves as a reference for setting up a CI/CD pipeline leveraging the following tools:

- **Docker** for containerizing applications.
- **Kubernetes** for orchestrating the deployment of Docker containers.
- **Helm** for Kubernetes package management.
- **ArgoCD** for declarative GitOps-based continuous delivery.

The pipeline integrates these tools to automate the build, test, and deploy phases of the application lifecycle.

![Architecture Diagram](./images/architecture.png) *(Include a diagram of your architecture)*

## Architecture

The architecture involves the following components:

- **Docker**: Used to containerize the application.
- **Kubernetes**: Orchestrates the deployment of Docker containers.
- **Helm**: Manages Kubernetes application deployment with Helm charts.
- **ArgoCD**: Manages deployment workflows in Kubernetes using GitOps principles.

## Prerequisites

Before getting started, ensure you have the following:

- **Docker**: Installed and running locally.
- **Kubernetes Cluster**: A local or cloud-based cluster (e.g., Minikube, GKE, EKS, AKS).
- **Helm**: Installed for managing Kubernetes applications.
- **ArgoCD**: Installed and set up for managing Kubernetes deployments via GitOps.
- **GitHub**: For hosting your code repository and triggering CI/CD pipelines.

## Setup and Installation

Follow these steps to set up the environment:

### 1. Clone the repository:

```bash
git clone https://github.com/Rekapost/devopsified-cicd-docker-helm-argocd-k8s.git
cd devopsified-cicd-docker-helm-argocd-k8s

2. Install Docker:
Follow the official Docker installation guide for your operating system.

3. Install Helm:
Install Helm by following the instructions here.

4. Set up Kubernetes:
You can use Minikube for a local Kubernetes cluster. Install it by following the guide here.

5. Install ArgoCD:
Follow the ArgoCD installation guide to deploy it on your Kubernetes cluster.

Usage
After setting up the prerequisites, here’s how you can use the project:

1. Build Docker Image:
You can build the Docker image for your application:

bash
docker build -t <your_image_name>:<tag> .
2. Deploy with Helm:
Use Helm to install the application on your Kubernetes cluster:

bash
helm install <release_name> ./helm
3. Sync with ArgoCD:
Once the application is deployed, you can use ArgoCD to manage the deployment:

bash
argocd app sync <app_name>
Configuration
Docker Configuration
The Dockerfile in the root directory is used to build your Docker image.
It is optimized for multi-stage builds to keep the image size minimal.
Helm Configuration
The helm/ directory contains the Helm charts used for deploying applications on Kubernetes.
Edit the values.yaml file for environment-specific configurations.
ArgoCD Configuration
The ArgoCD configuration ensures that all changes pushed to the Git repository are automatically reflected in the Kubernetes cluster.
The repository configuration can be customized in the ArgoCD UI or via the CLI.
Deployment
Once your local setup is ready and the application is built, follow these steps to deploy your app:

Commit and push your changes to your GitHub repository.
ArgoCD will automatically detect changes in the repository and deploy the updated application to Kubernetes.
Contributing
We welcome contributions to improve and expand this project. To contribute:

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes.
Commit your changes (git commit -am 'Add feature').
Push to the branch (git push origin feature-branch).
Create a pull request.
Please ensure that your code adheres to the project's coding standards and includes proper test coverage where necessary.

License
This project is licensed under the MIT License - see the LICENSE file for details.

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
