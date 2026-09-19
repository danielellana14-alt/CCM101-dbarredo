# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

This laboratory activity introduces cloud-native engineering and containerization using Docker. The activity focuses on understanding the differences between traditional Virtual Machines (VMs) and containers and demonstrates how Docker can be used to deploy and manage a containerized Nginx web server. The practical activities were performed using a Docker-enabled Ubuntu environment in the KillerCoda Playground.

## Objectives

The objectives of this laboratory activity are to:

* Differentiate between Virtual Machines and containers.
* Access and verify a Docker-enabled cloud environment.
* Execute fundamental Docker CLI commands.
* Pull and run a containerized Nginx web server.
* Map a host network port to a container port.
* Manage the lifecycle of a Docker container.
* Document container operations using Markdown.
* Maintain an organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Check Docker Installation

```bash
docker --version
```

Displays the installed Docker version.

### Check Docker Environment

```bash
docker info
```

Displays information about the Docker client, Docker server, storage, containers, images, and system environment.

### List Running Containers

```bash
docker ps
```

Displays currently running Docker containers.

### Pull Nginx

```bash
docker pull nginx
```

Downloads the official Nginx image from Docker Hub.

### Run Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

Runs the Nginx container in detached mode and maps host port 8080 to port 80 inside the container.

### Test Nginx

```bash
curl http://localhost:8080
```

Sends an HTTP request to the Nginx server and displays the returned webpage HTML.

### Stop Container

```bash
docker stop nginx-server
```

Stops the running Nginx container.

### View All Containers

```bash
docker ps -a
```

Displays running and stopped containers.

### Remove Container

```bash
docker rm nginx-server
```

Removes the Nginx container from the Docker environment.

## Skills Learned

Through this laboratory activity, I learned how to:

* Compare Virtual Machines and containers.
* Verify a Docker installation using the command line.
* Pull images from Docker Hub.
* Create and run Docker containers.
* Use detached mode to run services in the background.
* Configure Docker port mapping.
* Test a containerized web server using `curl`.
* Stop and remove Docker containers.
* Document technical procedures using Markdown.
* Organize laboratory evidence in a GitHub repository.

## Challenges Encountered

One challenge was becoming familiar with the Docker command-line interface and understanding the difference between Docker images and containers. Another challenge was understanding how port mapping connects the host machine's port 8080 to Nginx's port 80 inside the container. The activity also required careful documentation and screenshot organization to provide evidence for each checkpoint. After following the commands step by step, the Nginx container was successfully deployed, tested, stopped, and removed.
