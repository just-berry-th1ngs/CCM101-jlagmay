# Laboratory 07 - Cloud Operations Engineer

## Mission Overview

In this lab, I acted as a Cloud Operations Engineer at CloudNova Technologies. I checked the health of a Linux server, deployed an Nginx container, sent test traffic, and used logs and metrics to show the application is healthy.

## Objectives

- Use Linux commands to monitor CPU, memory, and disk.
- Deploy a web container and track it with Docker metrics.
- Generate web traffic and read the application logs.
- Write a technical report in Markdown.
- Add to my GitHub Cloud Computing Portfolio.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| `free -h` | Check total and used memory (RAM) |
| `df -h` | Check disk storage |
| `top` | View running processes and CPU load |
| `docker run -d --name client-website -p 8080:80 nginx` | Start the Nginx container |
| `docker ps` | Confirm the container is running |
| `curl http://localhost:8080` | Send a normal web request |
| `curl http://localhost:8080/hidden-admin-page` | Trigger a 404 error |
| `docker logs client-website` | Read the container logs |
| `docker stats` | View live CPU and memory use |

## Skills Learned

- Checking server health with Linux tools.
- Running a container in the background.
- Sending test requests with curl.
- Finding HTTP 200 and 404 codes in logs.
- Reading CPU and memory use of a container.
- Writing documentation in Markdown.

## Files

- [System Baseline Report](system-baseline-report.md)
- [Container Observability](container-observability.md)
- [Reflection](reflection.md)
