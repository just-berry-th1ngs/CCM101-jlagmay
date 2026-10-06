# Docker Compose Guide

## What does the `services:` block do?
(Points: it lists every container in the application. Each name under it,
`database` and `app`, is one service, and Compose creates one container
per service.)

## How did the app container find the database?
(Points: the `MYSQL_HOST=database` environment variable. Compose puts
all services on a shared network where each service name works as a
hostname, so `database` resolves to the MariaDB container.)

## `docker run` vs `docker-compose up -d`
(Points: `docker run` starts one container from a long command you type
each time. `docker-compose up -d` reads a YAML file and starts every
container, the network and the settings together, in the background,
and you can repeat it exactly.)
