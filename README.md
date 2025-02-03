# 🐳 Docker Workshop (Windows + Docker Desktop)

## 🚀 Overview
Welcome to the **Docker Workshop**! This guide will help you set up **Docker Desktop on Windows**, run containers, build custom images, and manage multi-container applications.

💻 **Prerequisites**
- Windows 10/11 with WSL2 enabled
- Docker Desktop installed (https://www.docker.com/products/docker-desktop)
- Basic knowledge of the terminal

---

## 📅 Workshop Agenda

### **1️⃣ Introduction to Docker**
- What is Docker?
- Containers vs. Virtual Machines
- Key Docker Concepts (Images, Containers, Volumes, Networks)
- Installing Docker Desktop on Windows (WSL2 vs. Hyper-V)

📌 **[Go to Section →](./01-introduction/README.md)**

---

### **2️⃣ Setting Up Docker on Windows**
- Install and Configure Docker Desktop
- Verify installation (`docker --version`, `docker info`)

📌 **[Go to Section →](./02-setup/README.md)**

---

### **3️⃣ Docker Basics**
- Running your first container (`docker run hello-world`)
- Managing containers (`docker ps`, `docker stop`, `docker rm`)
- Pulling images from Docker Hub (`docker pull nginx`)
- Writing a simple `Dockerfile`
- Building and running a custom image

📌 **[Go to Section →](./03-docker-basics/README.md)**

---

### **4️⃣ Docker Compose**
- What is Docker Compose?
- Writing a `docker-compose.yml` file
- Running multi-container apps (`docker-compose up -d`)

📌 **[Go to Section →](./04-docker-compose/README.md)**

---

### **5️⃣ Docker Volumes & Networking**
- Persisting data with Docker Volumes
- Creating and managing Docker Networks

📌 **[Go to Section →](./05-volumes-networks/README.md)**

---

### **6️⃣ Deploying Docker Containers**
- Tagging and pushing an image to Docker Hub
- Running containers on another machine

📌 **[Go to Section →](./06-deployment/README.md)**

---

## 🎯 Final Hands-on Challenge
Deploy a **Flask + PostgreSQL** app using Docker Compose!

📌 **[Go to Challenge →](./challenge/README.md)**

---

## 📚 Resources
- Official Docker Docs: [https://docs.docker.com/](https://docs.docker.com/)
- Play with Docker: [https://labs.play-with-docker.com/](https://labs.play-with-docker.com/)
- Docker Cheat Sheet: [https://dockerlabs.collabnix.com/docker/cheatsheet/](https://dockerlabs.collabnix.com/docker/cheatsheet/)

---

## 👨‍💻 How to Clone and Use This Repo
```sh
git clone https://github.com/YOUR_GITHUB/docker-workshop.git
cd docker-workshop
