# Docker Basic Commands

This file contains a list of basic Docker commands to help you get started with containerization.

## Table of Contents
1. [Docker Version](#docker-version)
2. [Run a Container](#run-a-container)
3. [List Running Containers](#list-running-containers)
4. [Stop a Container](#stop-a-container)
5. [Remove a Container](#remove-a-container)

### Docker Version
```bash
docker version
```

### Run a Container
```bash
docker run -it ubuntu /bin/bash
```

### List Running Containers
```bash
docker ps
```

### Build the image.
```bash
docker build -t <container_id> .
```

### Stop a Container
```bash
docker stop <container_id>
```

### Remove a Container
```bash
docker rm <the-container-id>
```

### Start an app container
#### The -d flag (short for --detach) runs the container in the background. 
#### The -p flag (short for --publish) creates a port mapping between the host and the container.
```bash
docker run -dp <host-port>:<container-port> <the-container-id>
```

### Create a volume 
```bash
docker volume create <volume-name>
```

### Start the container and mount volume
```bash
docker run -dp <host-port>:<container-port> <the-container-id> --mount type=volume,src=<volume-name>,target=<target-location>
```

### Inspect the volume
```bash
docker volume inspect <volume-name>
```

### Bind mount
```bash
docker run -it --mount type=bind,src="$(pwd)",target=/src ubuntu bash
```

### Create a network
```bash
docker network create <network-name>
```
 
### SSH into a running container
```bash
docker exec -it <container name> <command>
```

### Run the application stack
```bash
docker compose up -d
```
 