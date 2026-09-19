# Docker Deployment

## Nginx Container Deployment

The official Nginx Docker image was downloaded and used to deploy a web server container.

### 1. List Running Containers

```bash
docker ps
```

This command lists the Docker containers that are currently running.

### 2. Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container without removing it.

### 3. Verify the Container Is Stopped

```bash
docker ps
docker ps -a
```

The `docker ps` command confirms that the container is no longer running, while `docker ps -a` displays the stopped container and its status.

### 4. Remove the Container Completely

```bash
docker rm nginx-server
```

This command permanently removes the specified Docker container from the local Docker environment.

## Commands Used for Deployment

### Pull the Nginx Image

```bash
docker pull nginx
```

Downloads the official Nginx image from Docker Hub.

### Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

Creates and starts an Nginx container in detached mode and maps host port 8080 to port 80 inside the container.

### Test the Web Server

```bash
curl http://localhost:8080
```

Sends an HTTP request to the Nginx server and verifies that it returns the default Nginx webpage.

### Check Container Status

```bash
docker ps
```

Displays the currently running containers and their status.

## Container Lifecycle

The container was successfully created, started, tested, stopped, verified, and removed using Docker CLI commands.

