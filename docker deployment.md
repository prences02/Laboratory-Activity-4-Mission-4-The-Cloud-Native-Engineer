# Docker Deployment and Container Lifecycle

# 1. Download the Nginx Image

bash
docker pull nginx


This command downloads the official Nginx image from Docker Hub.

# 2. Run the Nginx Container

bash
docker run -d --name my-nginx -p 8080:80 nginx


This command starts Nginx in the background and maps host port 8080 to container port 80.

## 3. Verify the Web Server

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the local Nginx server and displays the returned HTML.

# 4. List Running Containers

bash
docker ps


This command displays all currently running containers.

## 5. Stop the Container

bash
docker stop my-nginx


This command gracefully stops the Nginx container.

# 6. Verify the Container Is Stopped

bash
docker ps


This command lists running containers and confirms that the stopped Nginx container is no longer running.

# 7. List All Containers

bash
docker ps -a


This command displays both running and stopped containers.

# 8. Remove the Container

bash
docker rm my-nginx


This command removes the stopped Nginx container from the Docker environment.

# Conclusion

Docker provides simple commands for deploying, inspecting, stopping, and removing containers. Understanding the container lifecycle helps engineers manage applications more efficiently.
