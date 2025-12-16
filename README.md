# CI/CD Pipeline using GitHub Actions + Docker + AWS EC2

## Overview
This project demonstrates a fully automated **CI/CD pipeline** for deploying applications using **GitHub Actions**, **Docker**, and **AWS EC2**. The pipeline automatically builds, tests, and deploys Dockerized applications to an EC2 instance whenever changes are pushed to the repository.

## Features
- Automated build and test workflow with **GitHub Actions**
- Docker containerization for consistent deployment
- Deployment to **AWS EC2** instance
- Continuous integration and continuous deployment for faster development cycles
- Easy configuration for multiple environments

## Technologies Used
- **GitHub Actions** – CI/CD automation
- **Docker** – Containerization
- **AWS EC2** – Deployment server
- **Bash / Shell Scripts** – Deployment automation

## Installation / Setup

### Prerequisites
- Docker installed locally
- AWS account with EC2 access
- GitHub repository

### Steps
1. **Clone the repository**
    ```bash
    git clone https://github.com/your-username/your-repo.git
    cd your-repo
    ```

2. **Configure AWS EC2**
    - Launch an EC2 instance
    - Set up SSH access
    - Install Docker on the EC2 instance

3. **Set up GitHub Actions**
    - Navigate to the `.github/workflows/` directory
    - Edit workflow YAML files with your EC2 instance IP, SSH key, and repository details

4. **Build and Run Docker Container Locally (Optional)**
    ```bash
    docker build -t your-app-name .
    docker run -p 80:80 your-app-name
    ```

5. **Push Changes**
    - Commit and push changes to GitHub
    - GitHub Actions will automatically build, test, and deploy to your EC2 instance

## Usage
- Access your deployed application via the EC2 public IP or domain.
- Modify the GitHub Actions workflow to customize deployment strategies or environments.





