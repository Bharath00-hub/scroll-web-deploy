# scroll-web-deploy 🚀

A responsive frontend web application forked and enhanced from [manjukolkar/scroll-web](https://github.com/manjukolkar/scroll-web), containerized with Docker, automated using Jenkins, and deployed to Kubernetes for scalable and efficient DevOps workflows.

##  Project Overview

This project demonstrates the deployment of a static website with modern DevOps practices including containerization, CI/CD, and cloud-native orchestration. The app structure is clean and modular, making it suitable for both personal learning and real-world use cases.

##  Key Features

- 🔹 Responsive web design using HTML, CSS, and JavaScript
- Dockerized for consistent cross-platform deployment
- Jenkins CI/CD pipeline with a `Jenkinsfile`
- Kubernetes deployment with `deploy.yaml`
- Organized asset management (CSS, JS, Fonts, Images)

## Tech Stack

| Category       | Tools / Technologies             |
|----------------|----------------------------------|
| Frontend       | HTML, CSS, JavaScript            |
| Containerization | Docker                         |
| CI/CD          | Jenkins                          |
| Orchestration  | Kubernetes                       |
| Version Control| Git, GitHub                      |

## Project Structure
scroll-web-deploy/
├── css/ # Stylesheets
├── fonts/ # Web fonts
├── images/ # Static images
├── js/ # JavaScript files
├── index.html # Main webpage
├── Dockerfile # Docker build instructions
├── Jenkinsfile # CI/CD pipeline config for Jenkins
└── deploy.yaml # Kubernetes deployment manifes

2. Run Locally
docker run -d -p 8080:80 scroll-web:latest

3. Setup CI/CD with Jenkins
Make sure Jenkins has Docker and GitHub plugins

Create a pipeline job pointing to this repo

Use the provided Jenkinsfile for build and deploy automation

4. Deploy to Kubernetes

kubectl apply -f deploy.yaml
kubectl get pods
kubectl get svc
