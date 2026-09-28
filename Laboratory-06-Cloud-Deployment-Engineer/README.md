# Laboratory 06 - The Cloud Deployment Engineer

## Mission Overview

Congratulations! Your flawless work in deploying data storage solutions has earned you a spot on the Cloud Deployment Team at CloudNova Technologies.

Up until now, you have been deploying single containers (like a standalone web server or a storage bucket). However, real-world enterprise applications are rarely just one container. They are "multi-tier" systems that require a frontend web application communicating seamlessly with a backend database. Deploying these one by one manually is prone to error.

Enter Docker Compose. In this mission, you will transition from manual commands to Infrastructure as Code (IaC). Using a YAML configuration file, you will define a multi-container private cloud storage application (Nextcloud and MariaDB) and deploy the entire stack simultaneously with a single command!

Remember: A junior engineer deploys servers by typing commands; a senior engineer deploys infrastructure by writing code.

## Mission Objectives

At the end of this laboratory activity, you should be able to:

- Explain the concept of a multi-tier application architecture.
- Understand the purpose and structure of a docker-compose.yml file.
- Use a Linux command-line text editor (nano) to create configuration files.
- Deploy a multi-container application (Nextcloud + Database) using Docker Compose.
- Document deployment procedures and Infrastructure as Code (IaC) principles using Markdown.
- Continue expanding your professional GitHub Cloud Computing Portfolio.

## Commands Executed

### Create the Deployment Directory

```bash
mkdir nextcloud-deployment
```

Creates a new directory for the Nextcloud deployment project.

### Enter the Deployment Directory

```bash
cd nextcloud-deployment
```

Moves into the Nextcloud deployment directory.

### Create the Docker Compose File

```bash
nano docker-compose.yml
```

Opens the nano text editor to create and edit the Docker Compose configuration file.

### Deploy the Multi-Container Stack

```bash
docker-compose up -d
```

Deploys the Nextcloud and MariaDB services in the background.

### Verify the Running Containers

```bash
docker-compose ps
```

Displays the status of the services managed by Docker Compose.

### Shut Down the Infrastructure

```bash
docker-compose down
```

Stops and removes the containers created by the Docker Compose deployment.

## Skills Learned

- Understanding multi-tier application architecture.
- Creating Docker Compose YAML configuration files.
- Using nano to create configuration files.
- Deploying multiple containers using Docker Compose.
- Connecting a Nextcloud application to a MariaDB database.
- Using environment variables in a Compose file.
- Understanding Infrastructure as Code (IaC).
- Using Git and GitHub to document cloud computing work.
