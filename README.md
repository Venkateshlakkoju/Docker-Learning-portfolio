# Docker Learning Portfolio 🐳

A hands-on Docker learning repository documenting my journey into containerization and DevOps.

I created these practical examples while learning Docker, building images, running containers, managing storage, and writing Dockerfiles.

## 📚 Concepts Practiced

- Docker images and containers
- Dockerfile instructions: `FROM`, `RUN`, `CMD`, `COPY`, `ADD`
- `WORKDIR` and `EXPOSE`
- Environment variables using `ENV` and `ARG`
- `ENTRYPOINT` vs `CMD`
- Docker volumes
- `.dockerignore`
- Image layers and build cache
- Multi-stage Docker builds

## 📁 Repository Structure

| Folder | Concept |
|---|---|
| `add-demo/` | ADD instruction |
| `arg-demo/` | Build-time ARG |
| `cached-image/` | Image layers and build cache |
| `dockerfile-basics/` | ENTRYPOINT and CMD |
| `dockerignore-demo/` | .dockerignore |
| `multi-stage-build/` | Multi-stage builds |
| `volume-demo/` | Docker VOLUME |
| `website/` | Sample website HTML |

## 🚀 Getting Started

Make sure Docker is installed and running.

Clone this repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd docker-learning-portfolio
```

Build and run an example:

```bash
docker build -t add-demo ./add-demo
docker run --rm add-demo
```

### Build the ARG example

```bash
docker build -t arg-demo ./arg-demo
docker build -t arg-demo:v2 --build-arg APP_VERSION=2.0 ./arg-demo
docker run --rm arg-demo:v2
```

### Build the multi-stage example

```bash
docker build -t multi-stage-demo ./multi-stage-build
docker run -d --name multi-stage-container -p 8087:80 multi-stage-demo
```

Open `http://localhost:8087` in your browser.

### Build the volume example

```bash
docker build -t volume-demo ./volume-demo
docker volume create docker-volume
docker run -d --name volume-container -v docker-volume:/app/data volume-demo
```

## 🎯 Learning Objective

The objective of this repository is to develop practical Docker skills and build a strong foundation for DevOps tools and workflows.

## 🛠️ Tools Used

- Docker
- Docker Desktop
- Ubuntu on WSL2
- Linux terminal
- Git and GitHub

## 📈 Next Learning Goals

- Docker Networking
- Docker Compose
- Container troubleshooting
- CI/CD
- Kubernetes

---

**Learning by doing, one container at a time!** 🚀
