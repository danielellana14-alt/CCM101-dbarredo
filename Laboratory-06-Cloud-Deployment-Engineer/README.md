# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

This laboratory focuses on deploying a multi-tier private cloud storage application using Docker Compose. The application uses Nextcloud as the web application and MariaDB as its database.

## Objectives

* Understand two-tier architecture.
* Create a Docker Compose YAML configuration.
* Deploy and manage multiple containers using Docker Compose.
* Access the Nextcloud web interface through a browser.
* Apply Infrastructure as Code (IaC) principles.
* Document deployment procedures using Markdown.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

* Docker Compose configuration
* Multi-tier application architecture
* Container deployment and management
* Linux command-line text editing
* Infrastructure as Code (IaC)
* Technical documentation using Markdown
* GitHub portfolio management

## Screenshots

The following screenshots provide evidence of the deployment process:

* `compose-deployment.png` - Successful deployment and running containers.
* `nextcloud-web.png` - Nextcloud web interface.
* `compose-teardown.png` - Containers stopped and removed successfully.

