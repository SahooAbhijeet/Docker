# Docker Commands Cheat Sheet

## 1. Check Docker Version
**Command:**  
```bash
docker --version
```
**Description:** Check the installed Docker version.

## 2. Display System-Wide Docker Info
**Command:**  
```bash
docker info
```
**Description:** Display system-wide information about Docker.

## 3. List Docker Images
**Command:**  
```bash
docker images
```
**Description:** List all available Docker images.

## 4. Pull a Docker Image
**Command:**  
```bash
docker pull nginx
```
**Description:** Download a Docker image from DockerHub.

## 5. Run a Docker Container
**Command:**  
```bash
docker run nginx
```
**Description:** Create and start a Docker container from an image.

## 6. List Running Containers
**Command:**  
```bash
docker ps
```
**Description:** List all running containers.

## 7. List All Containers
**Command:**  
```bash
docker ps -a
```
**Description:** List all containers (including stopped ones).

## 8. Start a Stopped Container
**Command:**  
```bash
docker start my_container
```
**Description:** Start a stopped container.

## 9. Stop a Running Container
**Command:**  
```bash
docker stop my_container
```
**Description:** Stop a running container.

## 10. Remove a Container
**Command:**  
```bash
docker rm my_container
```
**Description:** Remove a container.

## 11. Remove an Image
**Command:**  
```bash
docker rmi nginx
```
**Description:** Remove an image.

## 12. Build Image from Dockerfile
**Command:**  
```bash
docker build -t my_image .
```
**Description:** Build a Docker image from a Dockerfile.

## 13. Run Command Inside Container
**Command:**  
```bash
docker exec -it my_container /bin/bash
```
**Description:** Run a command inside a running container.

## 14. Display Container Logs
**Command:**  
```bash
docker logs my_container
```
**Description:** Display logs of a container.

## 15. Inspect a Container
**Command:**  
```bash
docker inspect my_container
```
**Description:** Display detailed information about a container.

## 16. List Docker Networks
**Command:**  
```bash
docker network ls
```
**Description:** List Docker networks.

## 17. Create Docker Network
**Command:**  
```bash
docker network create my_network
```
**Description:** Create a Docker network.

## 18. List Docker Volumes
**Command:**  
```bash
docker volume ls
```
**Description:** List Docker volumes.

## 19. Create Docker Volume
**Command:**  
```bash
docker volume create my_volume
```
**Description:** Create a Docker volume.

## 20. Prune System
**Command:**  
```bash
docker system prune
```
**Description:** Remove all stopped containers, unused networks, dangling images, and unused volumes.

## 21. Detached Mode Run
**Command:**  
```bash
docker run -d nginx
```
**Description:** Run a container in detached mode.

## 22. Port Mapping
**Command:**  
```bash
docker run -p 8080:80 nginx
```
**Description:** Map a container port to a host port.

## 23. Mount Host Directory
**Command:**  
```bash
docker run -v /host/path:/container/path nginx
```
**Description:** Mount a host directory as a volume inside the container.

## 24. Set Environment Variables
**Command:**  
```bash
docker run -e MYSQL_ROOT_PASSWORD=password mysql
```
**Description:** Set environment variables in the container.

## 25. Name a Container
**Command:**  
```bash
docker run --name my_container nginx
```
**Description:** Specify a custom name for the container.

## 26. Copy Files to Container
**Command:**  
```bash
docker cp index.html my_container:/usr/share/nginx/html/
```
**Description:** Copy files or directories between the host and the container.

## 27. Commit Container Changes
**Command:**  
```bash
docker commit my_container my_image:v2
```
**Description:** Create a new image from a container’s changes.

## 28. Tag Docker Image
**Command:**  
```bash
docker tag my_image:latest my_image:1.0
```
**Description:** Tag an image with a new name and/or tag.

## 29. Save Image to Tar File
**Command:**  
```bash
docker save -o my_image.tar my_image
```
**Description:** Save an image to a tar archive file.

## 30. Load Image from Tar File
**Command:**  
```bash
docker load -i my_image.tar
```
**Description:** Load an image from a tar archive file.

## 31. Docker Login
**Command:**  
```bash
docker login
```
**Description:** Log in to a Docker registry (e.g., DockerHub).

## 32. Docker Logout
**Command:**  
```bash
docker logout
```
**Description:** Log out from a Docker registry.

## 33. Push Image to Registry
**Command:**  
```bash
docker push my_username/my_image
```
**Description:** Push an image to a Docker registry.

## 34. Pull Image from Registry
**Command:**  
```bash
docker pull my_username/my_image
```
**Description:** Pull an image from a Docker registry.

## 35. Prune Unused Images
**Command:**  
```bash
docker image prune
```
**Description:** Remove unused images.

## 36. Prune Stopped Containers
**Command:**  
```bash
docker container prune
```
**Description:** Remove all stopped containers.

## 37. Prune Unused Volumes
**Command:**  
```bash
docker volume prune
```
**Description:** Remove unused volumes.

## 38. Prune Unused Networks
**Command:**  
```bash
docker network prune
```
**Description:** Remove unused networks.

## 39. Docker Disk Usage
**Command:**  
```bash
docker system df
```
**Description:** Display disk usage by Docker.

## 40. Resource Usage Stats
**Command:**  
```bash
docker stats
```
**Description:** Display live resource usage statistics for containers.

## 41. Container Processes
**Command:**  
```bash
docker top my_container
```
**Description:** Display running processes of a container.

## 42. Pause Container
**Command:**  
```bash
docker pause my_container
```
**Description:** Pause all processes within a container.

## 43. Unpause Container
**Command:**  
```bash
docker unpause my_container
```
**Description:** Unpause a paused container.

## 44. Restart Container
**Command:**  
```bash
docker restart my_container
```
**Description:** Restart a running container.

## 45. Execute Command in Container
**Command:**  
```bash
docker exec my_container ls -l /app
```
**Description:** Run a command inside a running container.

## 46. Attach to Container
**Command:**  
```bash
docker attach my_container
```
**Description:** Attach local standard input, output, and error streams to a running container.

## 47. Build Without Cache
**Command:**  
```bash
docker build --no-cache -t my_image .
```
**Description:** Build a Docker image without using cache.

## 48. Inspect Container State in JSON
**Command:**  
```bash
docker inspect --format '{{json .State}}' my_container
```
**Description:** Display detailed state information about a container in JSON format.

## 49. Real-Time Events
**Command:**  
```bash
docker events
```
**Description:** Get real-time events from the server.

## 50. Kill a Container
**Command:**  
```bash
docker kill my_container
```
**Description:** Kill a running container by sending a SIGKILL signal.