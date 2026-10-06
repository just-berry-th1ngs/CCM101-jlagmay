# Multi-Tier Architecture

## What is a Two-Tier Architecture?
An application split into two parts. One part is the web or application tier.
The other is the database tier. They talk to each other over a network.

## The Web/Application Tier
- Shows the user interface
- Receives HTTP requests from the browser
- Runs the application logic
- Asks the database for data

In this lab, this is the Nextcloud container.

## The Database Tier
- Stores data that must be kept, like user accounts and file information
- Answers requests from the web tier

In this lab, this is the MariaDB container.

## Why Separate Them?
Each container does one job, so it is easier to fix, update, and restart
one without affecting the other. The database is also safer because users
do not connect to it directly. If one container fails, we know where to
look.
