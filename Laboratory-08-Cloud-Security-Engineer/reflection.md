A host-based firewall protects the server by blocking unauthorized connections, even if attackers enter the network. For example, it can only be accessed via SSH from trusted IP addresses and other connections will be denied. This will provide an additional level of security for the server and its information.

Managing open network ports helps reduce the server's attack surface. For each open port that is not needed, attackers have one more way to access your system. For example, restricting access to SSH and port 8080 enables services required by server to be accessed in a smaller manner.

Leaving MySQL port 3306 open to the public internet exposes the database to password attacks and unauthorized access. The attackers could steal information of the customer or remove important information. Database connections should only be made from trusted application servers and trusted administrators.

This mission changed my view of server security. I learned how a small mistake, such as forgetting to configure firewall rules, creates security risks. I also learned to allow SSH before enabling UFW to avoid losing remote access. Checking firewall status and testing the web application helped me understand the importance of careful configuration.

My GitHub portfolio now contains eight completed cloud computing missions. Each activity was a great opportunity to practice Linux commands and gain more knowledge about cloud infrastructure. I also learned how to write mark down files, how to organize folders, and upload screenshots as evidence. This eighth mission helped me understand firewall rules and server protection. I still need more practice with Linux security commands, especially when checking ports and troubleshooting connection problems.
