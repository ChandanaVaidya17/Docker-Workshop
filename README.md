# 🚀 Docker Workshop (Windows - Docker Desktop)

## Workshop Overview
Docker basics, containerization, networking, and Docker Compose on Windows using Docker Desktop.


###  Introduction to Docker**
#### Topics Covered:
- What is Docker? Why use it?
- Containers vs. Virtual Machines
- Installing Docker Desktop (Windows)
- Understanding **WSL2 vs. Hyper-V**
- Running your first container

#### Hands-on:
```sh
docker --version   # Check installation
docker run hello-world  # Run first container
docker ps  # List running containers
docker images  # View downloaded images
docker info  # Docker system details
```

---

###  Working with Containers & Images**
#### Topics Covered:
- Pulling & Running Images (`docker pull nginx`)
- Container Lifecycle (`start`, `stop`, `rm`, `logs`)
- Inspecting Containers (`exec`, `inspect`)
- Writing a `Dockerfile` (Building Custom Images)
- Tagging & Pushing Images to Docker Hub

#### Hands-on:
```sh
docker pull nginx
docker run -d -p 8080:80 nginx

docker ps -a  # View all containers
docker logs <container_id>  # View logs
docker exec -it <container_id> sh  # Enter container
```
Creating a custom **Dockerfile**:
```dockerfile
FROM nginx:latest
COPY index.html /usr/share/nginx/html/index.html
```
Build & Run:
```sh
docker build -t my-nginx .
docker run -d -p 8080:80 my-nginx
docker tag my-nginx username/my-nginx
docker push username/my-nginx  # Push to Docker Hub
```

---

###  Volumes, Networking & Docker Compose**
#### Topics Covered:
- **Volumes & Persistent Storage**
- **Networking in Docker** (Creating custom networks)
- **Docker Compose** (Managing multiple containers)

#### Hands-on:
```sh
docker volume create mydata
docker run -d -v mydata:/data --name mycontainer alpine

docker network create mynetwork
docker run -d --net=mynetwork --name=web nginx
```

Using **Docker Compose**:
```yaml
version: '3'
services:
  web:
    image: nginx
    ports:
      - "8080:80"
  redis:
    image: redis
```
Run:
```sh
docker-compose up -d
docker-compose down
```

---

---

## 📖 **Resources & References**
- [Docker Documentation](https://docs.docker.com/)
- [Docker Hub](https://hub.docker.com/)
- [Docker Cheat Sheet](https://dockerlabs.collabnix.com/docker/cheatsheet/)

---

⚡ **Happy Dockering! **
