# Docker Deployment

## Container Lifecycle Commands

### 1. List Running Containers

```bash
docker ps
```

This command lists the Docker containers that are currently running.

### 2. Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

### 3. Verify the Container is Stopped

```bash
docker ps
```

This command verifies that the Nginx container is no longer running.

### 4. Remove the Container Completely

```bash
docker rm nginx-server
```

This command removes the stopped Nginx container completely.
