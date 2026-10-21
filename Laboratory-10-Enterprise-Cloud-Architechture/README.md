# Laboratory 10 - Enterprise Cloud Architect

## Mission Overview

In this lab, I acted as an Enterprise Cloud Architect at CloudNova Technologies. I designed and deployed a multi-tier application using Ghost and MySQL inside Docker containers on an Ubuntu Server virtual machine running in VirtualBox. I also configured persistent storage, secured the server with UFW, and automated database backups using a Bash script and cron job.

## Objectives

- Design a cloud infrastructure architecture diagram.
- Provision and configure an Ubuntu Server virtual machine.
- Deploy Ghost and MySQL using Docker and Docker Compose.
- Configure persistent volumes for database and application data.
- Secure the server using UFW and a default-deny incoming policy.
- Write a Bash script to automate database backups.
- Schedule automated backups using cron.
- Test database restoration and service recovery.
- Document the infrastructure and complete my GitHub Cloud Computing Portfolio.

## Technologies Used

- Ubuntu Server
- Oracle VirtualBox
- Docker and Docker Compose
- Ghost
- MySQL
- UFW Firewall
- Bash Scripting
- Cron Scheduling
- SSH
- Markdown and GitHub

## Commands Executed

| Command | Purpose |
|---|---|
| `ssh -p 2222 vin@127.0.0.1` | Connect to the Ubuntu Server VM |
| `docker compose pull` | Download the required container images |
| `docker compose up -d` | Deploy the application containers |
| `docker compose ps` | Check the container status |
| `docker compose down` | Stop and remove the containers without deleting persistent volumes |
| `sudo ufw status verbose` | Check firewall status and rules |
| `sudo ss -tulpn` | Check listening ports |
| `./automation-script.sh` | Run the automated database backup script |
| `ls -lh ~/backups` | Check generated backup files |
| `cat ~/backups/backup.log` | View the backup log |
| `crontab -l` | View scheduled cron jobs |
| `docker volume ls` | Check existing Docker volumes |
| `sudo reboot` | Restart the Ubuntu Server VM |

## Skills Learned

- Designing a multi-tier cloud infrastructure.
- Deploying connected containers using Docker Compose.
- Configuring persistent storage with Docker volumes.
- Managing Linux server security with UFW.
- Checking open ports and network services.
- Automating database backups using Bash.
- Scheduling recurring tasks using cron.
- Restoring database records from backup files.
- Testing container recovery after a server reboot.
- Documenting infrastructure deployment and maintenance in Markdown.

## Files

- [Architecture Diagram](architecture-diagram.png)
- [Docker Compose Configuration](docker-compose.yml)
- [Automation Script](automation-script.sh)
- [Operational Manual](operational-manual.md)
- [Final Reflection](final-reflection.md)

## Project Summary

This laboratory activity combined the Linux, virtualization, containerization, security, storage, and automation concepts learned throughout the CCM101 Cloud Computing course. The project demonstrates how to deploy, secure, maintain, and recover a containerized web application in a local cloud environment.
