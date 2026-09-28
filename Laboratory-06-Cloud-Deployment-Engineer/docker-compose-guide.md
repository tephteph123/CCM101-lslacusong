# Docker Compose Guide

The services: block defines the containers used in the deployment. The YAML file has two services, database and app. The database service uses MariaDB, while the app service uses Nextcloud.

The Nextcloud app container finds the database container through the MYSQL_HOST environment variable. The value is database, which matches the name of the database service in the Compose file. This tells Nextcloud where to connect for the MariaDB database.

The docker run command starts one Docker container using the settings given in the command. The docker-compose up -d command starts the services listed in the docker-compose.yml file in the background. In this setup, one command starts both the database and Nextcloud containers.
