Student Management API - DevOps CI Pipeline Project

Screenshots

A Spring Boot REST API application containerized with Docker and integrated with a GitHub Actions CI pipeline for automated build, Docker image creation, and Docker Hub publishing.

Project Overview
This project was created to gain hands-on experience with modern DevOps practices including:

Git & GitHub
Linux Administration
Maven Build Automation
Docker Containerization
GitHub Actions CI
Docker Hub Integration
The application is built using Spring Boot and deployed inside Docker containers.


Tech Stack

Backend
Java 21
Spring Boot
Maven


DevOps Tools
Git
GitHub
GitHub Actions
Docker
Docker Hub
Ubuntu Linux VM


Project Architecture
Developer
    │
    ▼
GitHub Repository
    │
    ▼
GitHub Actions
    │
    ├── Maven Build
    │
    ├── Docker Image Build
    │
    └── Docker Hub Push
    │
    ▼
Docker Hub
    │
    ▼
Ubuntu Virtual Machine
    │
    ▼
Docker Container
    │
    ▼
Running Spring Boot Application


CI Workflow
Whenever code is pushed to the main branch:

GitHub Actions workflow is triggered.
Maven builds the project.
Spring Boot JAR file is generated.
Docker image is created.
Docker image is pushed to Docker Hub automatically.


Docker Commands Used

Build Image
docker build -t student-api .

Run Container
docker run -d -p 8080:8080 --name student-api-v1 student-api

Check Running Containers
docker ps

View Logs
docker logs student-api-v1


CI Pipeline Validation
The pipeline was validated by:

Modifying source code
Pushing changes to GitHub
Triggering GitHub Actions automatically
Building a new Docker image
Publishing the image to Docker Hub
Pulling the updated image on Ubuntu Linux VM
Running the updated application successfully


Learning Outcomes
Through this project I gained hands-on experience with:

Linux Command Line
Git and GitHub
Maven Build Process
Docker Image Creation
Docker Container Management
GitHub Actions Workflows
CI Pipeline Troubleshooting
Docker Hub Integration


Future Improvements
Continuous Deployment (CD)
AWS EC2 Deployment
Kubernetes Deployment
Monitoring with Prometheus and Grafana
Infrastructure as Code using Terraform


Author
Madawa Vishwajith

LinkedIn: https://www.linkedin.com/in/madawa-vishwajith-5a78112a7/

GitHub: https://github.com/madawaMax
