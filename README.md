# docker-templates
Repository for centralized Docker Compose templates, configurations, and resources to streamline containerized application setup and deployment across projects

## Docker Cheatsheet

### Common Docker Commands

- `docker run [OPTIONS] IMAGE [COMMAND] [ARG...]`
  - Run a command in a new container
- `docker start [OPTIONS] CONTAINER [CONTAINER...]`
  - Start one or more stopped containers
- `docker stop [OPTIONS] CONTAINER [CONTAINER...]`
  - Stop one or more running containers
- `docker build [OPTIONS] PATH | URL | -`
  - Build an image from a Dockerfile
- `docker pull [OPTIONS] NAME[:TAG|@DIGEST]`
  - Pull an image or a repository from a registry
- `docker push [OPTIONS] NAME[:TAG]`
  - Push an image or a repository to a registry
- `docker exec [OPTIONS] CONTAINER COMMAND [ARG...]`
  - Run a command in a running container
- `docker logs [OPTIONS] CONTAINER`
  - Fetch the logs of a container
- `docker-compose up [OPTIONS] [SERVICE...]`
  - Build, (re)create, start, and attach to containers for a service
- `docker-compose down [OPTIONS]`
  - Stop and remove containers, networks, images, and volumes

### Advanced Docker Commands

- `docker inspect [OPTIONS] CONTAINER|IMAGE`
  - Return low-level information on Docker objects
- `docker stats [OPTIONS] [CONTAINER...]`
  - Display a live stream of container(s) resource usage statistics
- `docker network ls`
  - List all networks
- `docker volume ls`
  - List all volumes
- `docker system prune [OPTIONS]`
  - Remove unused data

### Dockerfile Best Practices

- Use multi-stage builds to reduce image size
- Always specify a version for the base image
- Use `.dockerignore` to exclude unnecessary files
- Minimize the number of layers in the Dockerfile
- Use `COPY` instead of `ADD` unless you need to extract a tar file

### Troubleshooting Tips

- Use `docker logs [CONTAINER]` to view container logs
- Use `docker exec -it [CONTAINER] /bin/bash` to access a running container
- Use `docker ps -a` to list all containers, including stopped ones
- Use `docker-compose logs [SERVICE]` to view logs for a specific service in a Docker Compose setup
- Use `docker system df` to view disk usage by Docker

### Docker Installation Guides

- [Docker Desktop for Mac](https://docs.docker.com/docker-for-mac/install/)
- [Docker Desktop for Windows](https://docs.docker.com/docker-for-windows/install/)
- [Docker Engine on Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
- [Docker Engine on CentOS](https://docs.docker.com/engine/install/centos/)
- [Docker Engine on Debian](https://docs.docker.com/engine/install/debian/)
- [Docker Engine on Fedora](https://docs.docker.com/engine/install/fedora/)
- [Docker Engine on Raspbian](https://docs.docker.com/engine/install/raspbian/)

### Popular Docker Sites and Resources

- [Docker Hub](https://hub.docker.com/)
- [Docker Documentation](https://docs.docker.com/)
- [Docker GitHub](https://github.com/docker)
- [Awesome Docker](https://github.com/veggiemonk/awesome-docker)
- [Play with Docker](https://labs.play-with-docker.com/)

### History of Docker

Docker was initially released in March 2013 by Solomon Hykes, as an internal project within dotCloud, a platform-as-a-service company. Docker's primary innovation was to make containers easy to use and portable, allowing developers to package applications and their dependencies into a single container that could run on any system with Docker installed. This solved many issues related to environment consistency and dependency management, making it easier to develop, test, and deploy applications.

Docker quickly gained popularity and became the de facto standard for containerization. In 2014, Docker Inc. was formed, and the company shifted its focus entirely to Docker. Over the years, Docker has continued to evolve, adding new features and integrations, and has become a cornerstone of modern DevOps practices and cloud-native application development.

### Related Apps

- [Portainer](https://www.portainer.io/): A powerful, open-source management UI for Docker.
- [Rancher](https://rancher.com/): An open-source platform for managing Kubernetes and Docker in production.
- [Kitematic](https://kitematic.com/): A simple application for managing Docker containers on Mac and Windows.
- [Watchtower](https://containrrr.dev/watchtower/): A process for automating Docker container base image updates.
- [LazyDocker](https://github.com/jesseduffield/lazydocker): A simple terminal UI for both Docker and Docker Compose.
