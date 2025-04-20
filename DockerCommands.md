
# 🐳 Docker Commands Cheat Sheet (with Examples & Images)

---

## 1. `docker ps`

> 🔍 Shows the process status of Docker — i.e., lists only the **running containers**.

**Example:**
```bash
docker ps
```

![docker ps output](https://via.placeholder.com/800x200?text=docker+ps+output)

---

## 2. `docker stop <container_id>`

> 🛑 Stops the Docker container with the specified container ID.

**Example:**
```bash
docker stop d9a45c27d61a
```

![docker stop output](https://via.placeholder.com/800x200?text=docker+stop+output)

---

## 3. `docker run -p 3000:3000 <image_id>`

> 🚀 Runs a Docker container with **port mapping** from host to container.

**Example:**
```bash
docker run -p 3000:3000 abc12345def
```

---

## 4. `docker image ls`

> 📦 Lists all the **Docker images** available on your system.

**Example:**
```bash
docker image ls
```

![docker image ls](https://via.placeholder.com/800x200?text=docker+image+ls+output)

---

## 5. `docker run -d -p 3000:3000 <image_id>`

> 🧠 Runs the container in **detached mode** (in the background), letting you use the same terminal for other commands.

**Example:**
```bash
docker run -d -p 3000:3000 abc12345def
```

---

## 6. `docker ps -a`

> 📋 Shows **all containers** (running + stopped).

**Example:**
```bash
docker ps -a
```

---

## 7. `docker rm <container_name>`

> 🗑️ Removes a specific Docker container.

**Example:**
```bash
docker rm my_container
```

---

## 8. `docker run -d --rm -p 3000:3000 <image_id>`

> 🧹 Automatically **removes the container** after it stops.

**Example:**
```bash
docker run -d --rm -p 3000:3000 abc12345def
```

---

## 9. `docker run -d --rm --name "mywebapp" -p 3000:3000 <image_id>`

> 🏷️ Assigns a **custom name** to your Docker container.

**Example:**
```bash
docker run -d --rm --name "mywebapp" -p 3000:3000 abc12345def
```

---

## 10. `docker build .`

> 🔨 Builds the Docker image using the Dockerfile in the current directory.

**Example:**
```bash
docker build .
```

---

## 11. `docker build -t <image_name>:<tag> .`

> 🏗️ Builds the Docker image and assigns a **name and version** and -t refers to **version**.

**Example:**
```bash
docker build -t mywebapp:1.0 .
```

---

## 12. `docker rmi <image_name>:<tag>`

> 🧽 Deletes the specified Docker image.

**Example:**
```bash
docker rmi mywebapp:1.0
```

---

📝 **Note**: Replace all `<image_id>`, `<container_id>`, `<image_name>`, and `<tag>` with your actual values.

📷 You can generate your own terminal screenshots or use placeholder image links like:

```
https://via.placeholder.com/800x200?text=your+image+description
```
and replace `"your+image+description"` with a meaningful name.

---