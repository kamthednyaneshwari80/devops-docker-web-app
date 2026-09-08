# Dockerized Web Application

A simple web application containerized using Docker and served with Nginx.

## 🚀 Project Overview

This project demonstrates how to package a web application into a Docker container and run it in an isolated and portable environment.

## 🛠️ Technology Stack

- HTML
- Docker
- Nginx
- Linux
- Git
- GitHub

## 🔄 Docker Workflow

```text
HTML Web Application
        ↓
    Dockerfile
        ↓
   Docker Image
        ↓
 Docker Container
        ↓
   Nginx Server
        ↓
 http://localhost:8080

🐳 Dockerfile

The application uses the official lightweight Nginx Alpine image.

 FROM nginx:alpine
COPY index.html /usr/share/nginx/html/index.html
EXPOSE 80

▶️ How to Run
Build Docker Image
docker build -t devops-docker-web-app .
Run Container
docker run -d -p 8080:80 --name docker-web-app devops-docker-web-app
Check Running Container
docker ps
Stop Container
docker stop docker-web-app
Start Container
docker start docker-web-app
View Logs
docker logs docker-web-app
🌐 Application

Open the application in your browser:

http://localhost:8080
🎯 Key Learnings
Docker image creation
Dockerfile configuration
Container lifecycle management
Port mapping
Nginx inside Docker
Docker logs and troubleshooting
Git and GitHub version control
📌 Project Status

✅ Docker image created
✅ Container running successfully
✅ Nginx serving the application
✅ Application tested on localhost:8080

👩‍💻 Author

Dnyaneshwari Kamthe