# Laboratory 04 - The Cloud-Native Engineer

## Mission Overview

Congratulations! After successfully guiding our clients through multi-cloud evaluations, you have been promoted to the Cloud-Native Engineering Team at CloudNova Technologies.

Modern cloud computing is no longer just about renting Virtual Machines (VMs) from AWS or Azure. Today's enterprise applications are built using lightweight, portable, and lightning-fast technologies called Containers.

Your new mission is to understand the shift from traditional virtualization to containerization.

Using the KillerCoda Playground, you will step into the shoes of a Cloud-Native Engineer. You will research the differences between VMs and containers, execute your very first Docker commands, and deploy a live, containerized web server in seconds.

Remember: A traditional system administrator manages servers, but a cloud-native engineer manages the services running on them.

## Mission Objectives

At the end of this laboratory activity, you should be able to:

- Differentiate between traditional Virtual Machines (VMs) and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI (Command Line Interface) commands.
- Pull, run, manage, and terminate a containerized application (Nginx).
- Create professional technical documentation of container operations using Markdown.
- Continue developing a well-organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### 1. Check Docker Version

```bash
docker --version
```

This command displays the installed Docker version and confirms that Docker is available.

### 2. Check Docker Information

```bash
docker info
```

This command displays detailed information about the Docker environment and its current status.

### 3. Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the official Nginx image from Docker Hub.

### 4. Run the Nginx Container

```bash
docker run -d -p 8080:80 --name nginx-server nginx
```

This command creates and runs an Nginx container in detached mode. The `-p 8080:80` maps port 8080 of the host machine to port 80 of the container.

### 5. Test the Nginx Web Server

```bash
curl http://localhost:8080
```

This command checks if the Nginx web server is running and accessible through localhost port 8080.

### 6. List Running Containers

```bash
docker ps
```

This command displays the Docker containers that are currently running.

### 7. Stop the Nginx Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container using its container name.

### 8. Verify the Container is Stopped

```bash
docker ps
```

This command verifies that the Nginx container is no longer running.

### 9. List All Containers

```bash
docker ps -a
```

This command displays all Docker containers, including running and stopped containers.

### 10. Remove the Nginx Container

```bash
docker rm nginx-server
```

This command permanently removes the stopped Nginx container.

### 11. Verify Container Removal

```bash
docker ps -a
```

This command verifies that the Nginx container has been removed from the container list.

## Skills Learned

- Understanding the difference between Virtual Machines and Containers.
- Using basic Docker CLI commands.
- Pulling and running a Docker image.
- Deploying an Nginx web server.
- Using port mapping.
- Managing the container lifecycle.
- Creating technical documentation using Markdown.
- Using Git and GitHub to maintain a cloud computing portfolio.

## Challenges Encountered

One challenge I encountered was understanding the difference between Virtual Machines and Containers. I also needed to understand how port mapping works when running the Nginx web server. Another challenge was remembering the correct Docker commands for stopping and removing a container. Practicing each command in KillerCoda helped me understand the process better.
