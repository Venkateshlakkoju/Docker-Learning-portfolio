# Docker Learning Portfolio 🐳

A hands-on Docker learning repository documenting my journey into containerization and DevOps.

This repository contains practical exercises, Dockerfiles, Docker Compose projects, networking examples, security practices, and container management tasks completed during my DevOps learning journey.

## 📚 Concepts Practiced

### Docker Fundamentals
- Docker images and containers
- Container lifecycle management
- Docker commands and troubleshooting

### Dockerfile and Image Creation
- FROM, RUN, CMD, COPY, ADD
- WORKDIR and EXPOSE
- ENV and ARG
- ENTRYPOINT vs CMD
- USER instruction
- .dockerignore
- Image layers and build cache
- Multi-stage builds
- Image tagging and custom image creation

### Docker Storage
- Docker volumes
- Bind mounts
- Persistent data management

### Docker Networking
- Bridge networks
- Custom bridge networks
- Container-to-container communication
- Docker DNS and service discovery
- Network isolation and reconnection

### Docker Compose
- Compose YAML files
- Multi-container applications
- Service dependencies
- Health checks
- Restart policies
- Networking and scaling
- Environment variables
- WordPress and MySQL final project

### Docker Security
- Running containers as non-root users
- Docker security best practices
- Secure environment variable handling

### Docker Hub
- Building and tagging images
- Pushing images to Docker Hub
- Public and private repositories

### Resource Management and Advanced Operations
- Container memory limits
- CPU resource management
- Container inspection and troubleshooting

## 📁 Repository Structure

| Folder | Concept |
|---|---|
| add-demo/ | ADD instruction |
| arg-demo/ | Build-time ARG |
| cached-image/ | Build cache |
| dockerfile-basics/ | ENTRYPOINT and CMD |
| dockerignore-demo/ | .dockerignore |
| multi-stage-build/ | Multi-stage builds |
| volume-demo/ | Docker volumes |
| website/ | Sample website |
| docker-compose/ | Docker Compose projects |
| docker-security/ | Docker security |
| docker-custom-image/ | Custom Docker image |
| Screenshorts/ | Practice screenshots |

## 🚀 Getting Started

Make sure Docker is installed and running.

Clone this repository:

    git clone https://github.com/Venkateshlakkoju/Docker-Learning-portfolio.git
    cd Docker-Learning-portfolio

Build and run an example:

    docker build -t add-demo ./add-demo
    docker run --rm add-demo

## 🐳 Docker Compose Examples

Navigate to a project folder and start its services:

    cd docker-compose/basic
    docker compose up -d --build

Check running services:

    docker compose ps

Stop and remove the containers and network:

    docker compose down

Note: Named volumes are preserved when using docker compose down without the -v option.

## 🔐 Environment Variables

Some Compose projects use environment variables for passwords and configuration.

Copy the example environment file before starting those projects:

    cp .env.example .env

Use your own local values in .env. Never commit real passwords, tokens, or secrets to GitHub.

## 🛠️ Tools Used

- Docker
- Docker Desktop
- Ubuntu on WSL2
- Linux terminal
- Git and GitHub
- Docker Hub

## 📈 Next Learning Goals

- CI/CD pipelines
- Kubernetes
- Advanced DevOps workflows

---

**Learning by doing, one container at a time!** 🚀
