# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview
In this mission I used Docker Compose to deploy a two-tier private cloud
storage application, Nextcloud (web tier) with MariaDB (database tier),
using a single YAML file and a single command, on a KillerCoda playground.

## Objectives
- Explain multi-tier application architecture
- Understand the purpose and structure of a `docker-compose.yml` file
- Create configuration files with the `nano` text editor
- Deploy a multi-container application with Docker Compose
- Document the procedure and Infrastructure as Code principles in Markdown
- Continue building my GitHub Cloud Computing Portfolio

## Commands Executed
```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned
- Writing a multi-container setup as code (YAML)
- Deploying and tearing down a whole stack with one command
- Connecting containers by service name
- Using environment variables to configure containers
- Troubleshooting directory errors with Compose

## Files in This Folder
- `multi-tier-architecture.md`
- `docker-compose-guide.md`
- `reflection.md`
- `screenshots/`
