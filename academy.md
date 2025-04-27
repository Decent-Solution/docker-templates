# Docker Academy Overview

## Introduction
Docker is a platform for developing, shipping, and running applications inside containers. Containers are lightweight, portable, and consistent across different environments.

## Key Concepts
- **Image**: A lightweight, standalone, and executable software package that includes everything needed to run a piece of software.
- **Container**: A runtime instance of an image. It includes the application and its dependencies.
- **Dockerfile**: A text file that contains instructions for building a Docker image.
- **Docker Compose**: A tool for defining and running multi-container Docker applications using a `docker-compose.yml` file.

## Common Docker Commands
- `docker run [OPTIONS] IMAGE [COMMAND] [ARG...]`: Run a command in a new container.
- `docker start [OPTIONS] CONTAINER [CONTAINER...]`: Start one or more stopped containers.
- `docker stop [OPTIONS] CONTAINER [CONTAINER...]`: Stop one or more running containers.
- `docker build [OPTIONS] PATH | URL | -`: Build an image from a Dockerfile.
- `docker pull [OPTIONS] NAME[:TAG|@DIGEST]`: Pull an image or a repository from a registry.
- `docker push [OPTIONS] NAME[:TAG]`: Push an image or a repository to a registry.
- `docker exec [OPTIONS] CONTAINER COMMAND [ARG...]`: Run a command in a running container.
- `docker logs [OPTIONS] CONTAINER`: Fetch the logs of a container.
- `docker-compose up [OPTIONS] [SERVICE...]`: Build, (re)create, start, and attach to containers for a service.
- `docker-compose down [OPTIONS]`: Stop and remove containers, networks, images, and volumes.

## Advanced Docker Commands
- `docker inspect [OPTIONS] CONTAINER|IMAGE`: Return low-level information on Docker objects.
- `docker stats [OPTIONS] [CONTAINER...]`: Display a live stream of container(s) resource usage statistics.
- `docker network ls`: List all networks.
- `docker volume ls`: List all volumes.
- `docker system prune [OPTIONS]`: Remove unused data.

## Dockerfile Best Practices
- Use multi-stage builds to reduce image size.
- Always specify a version for the base image.
- Use `.dockerignore` to exclude unnecessary files.
- Minimize the number of layers in the Dockerfile.
- Use `COPY` instead of `ADD` unless you need to extract a tar file.

## Troubleshooting Tips
- Use `docker logs [CONTAINER]` to view container logs.
- Use `docker exec -it [CONTAINER] /bin/bash` to access a running container.
- Use `docker ps -a` to list all containers, including stopped ones.
- Use `docker-compose logs [SERVICE]` to view logs for a specific service in a Docker Compose setup.
- Use `docker system df` to view disk usage by Docker.

## Popular Docker Sites and Resources
- Docker Hub
- Docker Documentation
- Docker GitHub
- Awesome Docker
- Play with Docker

## Related Apps
- Portainer: A powerful, open-source management UI for Docker.
- Rancher: An open-source platform for managing Kubernetes and Docker in production.
- Kitematic: A simple application for managing Docker containers on Mac and Windows.
- Watchtower: A process for automating Docker container base image updates.
- LazyDocker: A simple terminal UI for both Docker and Docker Compose.
