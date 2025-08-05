# 🚀 Escape the Wastage: A Beginner’s Guide to Docker and Containerization

Are you concerned about wasting compute resources, underutilized VMs, or high cloud bills? Still paying for servers that aren’t used to their full potential?

This project introduces you to the world of **Docker** and **containerization**, enabling you to run your Java applications in lightweight containers, saving cost and improving efficiency.

---

## 📘 What You'll Learn

- What are containers and why they matter
- How containers compare to virtual machines (VMs)
- Understanding Docker as a containerization platform
- Overview of Docker architecture and lifecycle
- How to write a `Dockerfile`
- How to build and run a Docker container for a simple Java application

---

## 🧱 Before Containers: Virtual Machine Era

VMs virtualize physical servers, allowing multiple operating systems to run on a single machine using a **hypervisor**. However, they still carry a lot of overhead (entire OS, duplicate dependencies, etc.), which leads to inefficiencies.

---

## 📦 Containers: Lightweight & Efficient

Containers solve this problem by:

- Sharing the host OS kernel
- Packaging the application, dependencies, and system libs
- Running isolated processes efficiently

Think of them as **lightweight, portable zip files for apps** — they start fast and consume fewer resources.

---

## 🐳 What is Docker?

[Docker](https://www.docker.com/) is a popular open-source containerization platform that allows you to:

- Define your environment using a `Dockerfile`
- Build repeatable images
- Run containers anywhere
- Push and pull images from Docker registries like [DockerHub](https://hub.docker.com/)

---

## 🧰 Docker Architecture Overview

| Component      | Description                                  |
|----------------|----------------------------------------------|
| Docker CLI     | User interface for running Docker commands   |
| Docker Daemon  | Core engine managing containers & images     |
| Dockerfile     | Instructions to build a Docker image         |
| Image          | Blueprint of your application                |
| Container      | Running instance of the image                |
| Registry       | Stores and shares container images           |

---

## 🔁 Docker Lifecycle

1. Write a `Dockerfile`
2. Build the image using `docker build`
3. Run a container from the image
4. Optionally push to/pull from a registry

---

## 🧪 Hands-On Project: Dockerizing a Java App

> This repository contains:
> - `Main.java` – A simple Java program
> - `Dockerfile` – Instructions to build a Docker image

---

## 🖥️ Local Setup Instructions

### ✅ Prerequisites
- [Docker Desktop](https://www.docker.com/products/docker-desktop) installed and running

### 🔧 Steps
```bash
git clone https://github.com/<your-username>/docker-project
cd docker-project
docker build -t my-java-app .
docker run my-java-app
