# Laboratory 04: The Cloud-Native Engineer

## Mission Overview

CloudNova's client was running its web apps on virtual machines that were slow to start and used a lot of RAM. My job was to show why containers are a better fit. I researched how VMs and containers differ, then used Docker to deploy an Nginx web server and manage it from start to finish.

## Objectives

1. Explain the main differences between virtual machines and containers.
2. Check that Docker is installed and working.
3. Pull an image from Docker Hub.
4. Run a container in the background and map a host port to it.
5. Test that the deployed web server responds.
6. Manage the container lifecycle: list, stop, and remove it.

## Docker Commands Executed

```bash
# Checkpoint 3: Check the Docker setup
docker --version                                   # Show the installed Docker version
docker info                                        # Show details about the Docker setup

# Checkpoint 4: Deploy Nginx
docker pull nginx                                  # Download the Nginx image from Docker Hub
docker run -d -p 8080:80 --name my-nginx nginx     # Start Nginx in the background, host port 8080 -> container port 80
curl http://localhost:8080                         # Check that Nginx answers on port 8080

# Checkpoint 5: Container lifecycle
docker ps                                          # List running containers
docker stop my-nginx                               # Stop the container
docker ps -a                                       # List all containers, including stopped ones
docker rm my-nginx                                 # Delete the stopped container
```

## Skills Learned

- Explaining the difference between VMs and containers in simple terms
- Checking a Docker install with `docker --version` and `docker info`
- Pulling images from Docker Hub
- Running a container in the background with `-d` and giving it a name with `--name`
- Mapping a host port to a container port with `-p`
- Testing a web server from the terminal with `curl`
- Reading container status with `docker ps` and `docker ps -a`
- Stopping and removing containers

## Challenges Encountered

- **Port mapping:** At first, `-p 8080:80` was confusing. It means port 8080 on my machine goes to port 80 inside the container, so I open `localhost:8080`, not port 80.
- **Stopped containers:** After `docker stop`, the container was gone from `docker ps`. I had to use `docker ps -a` to see it as `Exited`, and `docker rm` to delete it for good.

## Lab Files

- [Virtualization vs. Containers](virtualization-vs-containers.md)
- [Docker Deployment: Nginx](docker-deployment.md)
- [Reflection](reflection.md)
