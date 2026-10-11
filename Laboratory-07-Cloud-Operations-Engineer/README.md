# Mission 7: The Cloud Operations Engineer

## Mission Overview

Congratulations! Your ability to deploy multi-tier architectures has proven your technical capabilities. You have now been promoted to the Cloud Operations Team (often referred to in the industry as Site Reliability Engineering, or SRE) at CloudNova Technologies.

Deploying a cloud application is only the first step; keeping it running smoothly is the real challenge. When a server crashes or a web page takes ten seconds to load, you cannot simply guess what is wrong. You must rely on Observability and Monitoring to see inside your infrastructure.

Using the KillerCoda Playground, you will step into the role of a Cloud Operations Engineer. You will establish a performance baseline for your Linux server, deploy a containerized application, generate artificial web traffic, and hunt down performance metrics and system logs to prove the application is healthy.

Remember: A developer hopes the application works; a Site Reliability Engineer uses metrics and logs to prove it.

## Objectives

At the end of this laboratory activity, you should be able to:

- Utilize native Linux command-line tools to monitor host CPU, Memory, and Disk capacity.
- Deploy a web container and track its real-time performance using Docker metrics.
- Generate web traffic and extract application access logs for analysis.
- Translate raw performance data into a readable technical report using Markdown.
- Continue expanding a professional GitHub Cloud Computing Portfolio.

## Monitoring Commands Executed

- `free -h` — Check memory usage.
- `df -h /` — Check root file system storage.
- `top` — Monitor CPU load and running processes.
- `docker run -d --name client-website -p 8080:80 nginx` — Deploy the Nginx container.
- `curl http://localhost:8080` — Send HTTP requests to the web server.
- `curl http://localhost:8080/hidden-admin-page` — Generate a 404 response.
- `docker logs client-website` — View application logs.
- `docker stats` — Monitor container resource usage.

## Skills Learned

- Monitoring Linux server memory, disk, and CPU.
- Deploying a containerized Nginx web server.
- Generating HTTP requests and identifying HTTP errors.
- Analyzing Docker logs and container metrics.
- Recording technical findings using Markdown.
- Maintaining a GitHub Cloud Computing Portfolio.
