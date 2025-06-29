# 🚀 Task Tracker - DevOps

This repository manages the DevOps setup for the Task Tracker application, including CI/CD workflows and Docker-based deployment.

## 📦 Structure

- **task-tracker-backend**: FastAPI backend (as a submodule)
- **task-tracker-frontend**: React frontend (as a submodule)
- **.github/workflows**: CI/CD pipeline using GitHub Actions
- **docker-compose.yml**: Multi-container setup for backend and frontend


![image](https://github.com/user-attachments/assets/38aedd6e-0383-4737-a552-34a291c3e666)

## 🔄 CI/CD Workflow

Every push to the `master` branch triggers a GitHub Actions workflow that:

- Checks out code and submodules  
- Builds Docker images for both frontend and backend  
- Pushes images to Docker Hub
- **docker-compose up**

Make sure your repository has `DOCKER_USERNAME` and `DOCKER_PASSWORD` secrets configured.

## 🐳 Deployment

To run the entire system locally, use Docker Compose. It pulls the latest Docker images and starts both services automatically.

---
