# Docker Compose Guide

## 1. What Does the `services:` Block Do?

The `services:` block defines the containers that make up an application. In this laboratory, it defines two services: `database`, which runs MariaDB, and `app`, which runs Nextcloud.

## 2. How Does Nextcloud Find the Database?

The environment variable `MYSQL_HOST=database` tells Nextcloud where to find the MariaDB service. Docker Compose creates a shared network for the services, allowing Nextcloud to connect to the database using the service name `database`.

## 3. Docker Run vs. Docker Compose

The `docker run` command is commonly used to create and start an individual container by specifying its configuration through command-line options. In contrast, `docker-compose up -d` reads the `docker-compose.yml` file and starts all the defined services in the background, making multi-container deployments easier to manage and repeat.

## 4. Important Docker Compose Commands

* `docker-compose up -d` — Starts the services in the background.
* `docker-compose ps` — Displays the status of the containers.
* `docker-compose logs` — Displays service logs.
* `docker-compose down` — Stops and removes the containers and the default network.

## Conclusion

Docker Compose simplifies multi-container deployment by keeping the infrastructure configuration in one YAML file. This improves consistency, maintainability, and the ability to reproduce deployments.
