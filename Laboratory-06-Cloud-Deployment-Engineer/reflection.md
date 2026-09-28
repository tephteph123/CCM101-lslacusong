# Mission Reflection

Docker Compose made my work easier because I could place the configuration for several services in one docker-compose.yml file. Instead of entering many Docker commands separately. For example, a Nextcloud setup needs services such as Nextcloud and MySQL. Compose starts these services with the correct settings and connections.

YAML uses indentation to organize information, so spacing matters. If I use a Tab instead of Spaces, Docker Compose may report a YAML parsing error and stop the deployment. A small indentation mistake therefore affects the whole configuration. This taught me to check formatting before running a deployment.

We used environment variables such as MYSQL_PASSWORD to separate configuration values from the main Compose file. Variables also make the setup easier to change when different values are needed. Passwords and other credentials need careful handling, especially when working with GitHub repositories.

Deploying Nextcloud in a few minutes felt satisfying because I saw several services work together as one system. I also gained more confidence after seeing the storage platform running with containers. The activity showed me how automation saves time during deployment.

Since Mission 1, my understanding of Cloud Computing has become more practical. Before, I mainly understood cloud computing as online storage and remote servers. Now I understand how Linux, containers, networks, storage, databases, YAML files, and environment variables work together. I also learned that cloud engineers need careful configuration, troubleshooting, and documentation. Each task gave me hands-on experience with tools used to deploy and manage services.
