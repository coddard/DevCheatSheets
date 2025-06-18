# 🐳 Docker Cheat Sheet

**A colorful guide to Docker commands for developers who love containers 🌟**

---

## ▶️ Running Containers

| Command                      | Emoji | Description                          |
| ---------------------------- | ----- | ------------------------------------ |
| `docker run <image>`         | 🚀    | Start a new container from an image  |
| `docker run -it <image>`     | 💻    | Start container in interactive mode  |
| `docker run --rm <image>`    | 🧹    | Auto-delete container after exit     |
| `docker create <image>`      | 📦    | Create container without starting it |
| `docker start <container>`   | ⏯️    | Start a stopped container            |
| `docker stop <container>`    | ⏹️    | Gracefully stop container            |
| `docker kill <container>`    | 💀    | Force-kill container                 |
| `docker restart <container>` | 🔁    | Restart container                    |
| `docker pause <container>`   | ⏸️    | Suspend container processes          |
| `docker unpause <container>` | ▶️    | Resume paused container              |
| `docker rm <container>`      | 🗑️    | Delete container                     |

---

## 🧼 Container Bulk Management

| Command                                | Emoji | Description                 |
| -------------------------------------- | ----- | --------------------------- |
| `docker stop $(docker ps -q)`          | ⏹️    | Stop all running containers |
| `docker kill $(docker ps -a -q)`       | 💀    | Kill all containers         |
| `docker rm $(docker ps -a -q)`         | 🗑️    | Delete all containers       |
| `docker rm -vf $(docker ps -a -q)`     | 💥    | Delete containers + volumes |
| `docker rmi -f $(docker images -a -q)` | 🧨    | Delete all images           |
| `docker system prune`                  | 🧹    | Clean dangling data         |
| `docker system prune -a`               | 🧼    | Clean all unused data       |

---

## 🔍 Inspect Containers

| Command                      | Emoji | Description                 |
| ---------------------------- | ----- | --------------------------- |
| `docker ps`                  | 📋    | List running containers     |
| `docker ps --all`            | 📋    | List all containers         |
| `docker logs <container>`    | 📜    | Show container logs         |
| `docker logs -f <container>` | 🔍    | Follow container logs       |
| `docker top <container>`     | 📊    | List processes in container |
| `docker inspect <container>` | 🔎    | Show container details      |
| `docker diff <container>`    | 🆕    | Show filesystem changes     |

---

## 🛠️ Executing Commands

| Command                          | Emoji | Description                 |
| -------------------------------- | ----- | --------------------------- |
| `docker attach <container>`      | 🔗    | Attach to running container |
| `docker cp <container>:<path> .` | 📤    | Copy files from container   |
| `docker exec -it <container> sh` | 💬    | Run shell in container      |
| `docker wait <container>`        | ⏳    | Wait for container to exit  |

---

## 📦 Images

| Command                            | Emoji | Description                 |
| ---------------------------------- | ----- | --------------------------- |
| `docker image ls`                  | 📦    | List local images           |
| `docker history <image>`           | 🕰️    | Show image build history    |
| `docker pull <image>`              | 📥    | Pull image from registry    |
| `docker push <image>`              | 📤    | Push image to registry      |
| `docker tag <image> <tag>`         | 🏷️    | Tag an image                |
| `docker commit <container> <img>`  | 📸    | Create image from container |
| `docker save <image> > backup.tar` | 💾    | Export image as tarball     |
| `docker load < backup.tar`         | 📥    | Import image from tarball   |

---

## 🗂️ Volumes

| Command                          | Emoji | Description           |
| -------------------------------- | ----- | --------------------- |
| `docker volume ls`               | 📁    | List all volumes      |
| `docker volume create <volume>`  | 📁    | Create new volume     |
| `docker volume inspect <volume>` | 🔎    | Show volume details   |
| `docker volume rm <volume>`      | 🗑️    | Delete volume         |
| `docker volume prune`            | 🧹    | Delete unused volumes |

---
