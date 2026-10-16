# Mission 8: The Cloud Security Engineer

## Mission Overview

Congratulations! Your proactive approach to system monitoring has earned you a spot on the elite Cloud Security Team at CloudNova Technologies.

In the cloud, leaving a server unsecured for even a few minutes can lead to automated brute-force attacks and data breaches. Your mission today applies the security concepts you learned in Chapter 8. You will implement the principle of defense in depth by locking down a live server using a host-based firewall.

Using the KillerCoda Playground, you will step into the role of a Cloud Security Engineer. You will deploy a web application, audit the server's open ports, and configure the Uncomplicated Firewall (UFW) to block malicious traffic while allowing legitimate users to access the application.

Remember: Security is not a product you buy; it is a continuous process you maintain.

## Objectives

At the end of this laboratory activity, you should be able to:

- Understand the concept of the Attack Surface and the Principle of Least Privilege (PoLP).
- Perform a basic security audit of active network ports on a Linux server.
- Configure the Uncomplicated Firewall (UFW) with a Default Deny policy.
- Implement granular port management to selectively allow SSH and HTTP traffic.
- Document firewall rules and security best practices using Markdown.
- Continue expanding your professional GitHub Cloud Computing Portfolio.

## Commands Executed

- `docker run -d --name secure-web-app -p 8080:80 nginx` — Deploy the Nginx web application.
- `curl http://localhost:8080` — Test the web application.
- `sudo ufw allow ssh` — Allow SSH connections.
- `sudo ufw default deny incoming` — Deny incoming connections by default.
- `sudo ufw default allow outgoing` — Allow outgoing connections.
- `sudo ufw enable` — Activate the firewall.
- `sudo ufw status verbose` — Check firewall status and policies.
- `sudo ufw allow 8080/tcp` — Allow TCP traffic on port 8080.
- `sudo ufw status numbered` — Display numbered firewall rules.

## Skills Learned

- Understanding the Principle of Least Privilege and attack surface.
- Auditing server security and network ports.
- Configuring UFW firewall rules.
- Applying a Default Deny policy.
- Allowing SSH and web application traffic.
- Documenting security configurations using Markdown.
- Maintaining a GitHub Cloud Computing Portfolio.
