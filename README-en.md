# Docker Commands Quick Reference

This README provides a quick reference to the most common and useful Docker commands, helping in the management of containers, images, volumes, networks, and other Docker resources.

## Docker Version

Check the installed Docker version.

```bash
docker --version
```

## Container Management

### List Containers

List all active containers.

```bash
docker ps
```

List all containers, including inactive ones.

```bash
docker ps -a
```

### Run Container

Run a container from an image.

```bash
docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
```

Example:

```bash
docker run -d -p 80:80 --name webserver nginx
```

### Stop Container

Stop a running container.

```bash
docker stop CONTAINER_ID
```

### Start Container

Start a stopped container.

```bash
docker start CONTAINER_ID
```

### Remove Container

Remove a specific container.

```bash
docker rm CONTAINER_ID
```

Remove all stopped containers.

```bash
docker container prune
```

## Image Management

### List Images

List all local images.

```bash
docker images
```

### Build Image

Build an image from a Dockerfile.

```bash
docker build -t TAG .
```

### Remove Image

Remove a local image.

```bash
docker rmi IMAGE_ID
```

## Docker Compose

### Run Docker Compose

Start services defined in `docker-compose.yml`.

```bash
docker-compose up
```

Start in 'detached' mode (in the background).

```bash
docker-compose up -d
```

### Stop Docker Compose

Stop services run via Docker Compose.

```bash
docker-compose down
```

## Volumes

### List Volumes

Display all created volumes.

```bash
docker volume ls
```

### Create Volume

Create a new volume.

```bash
docker volume create VOLUME_NAME
```

### Remove Volume

Remove a specific volume.

```bash
docker volume rm VOLUME_NAME
```

## Networks

### List Networks

List all Docker networks.

```bash
docker network ls
```

### Create Network

Create a new network.

```bash
docker network create NETWORK_NAME
```

### Remove Network

Remove a specific network.

```bash
docker network rm NETWORK_NAME
```

---
