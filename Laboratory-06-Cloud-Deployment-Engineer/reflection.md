# Mission 6 Reflection

Writing a docker-compose.yml file makes a cloud engineer's job easier
because everything is in one file. Instead of typing a long command for
each container, I ran one command and both containers started. The file
can be reused, shared, and fixed easily. It is also easier to repeat the
same setup every time. This saves time and lowers mistakes.

If there is an indentation error, like using a Tab instead of spaces,
Docker Compose cannot read the YAML file. It shows an error and the
deployment does not start. That is why I used spaces only and checked the
file with the cat command.

We used environment variables like MYSQL_PASSWORD to set the database
name, user, and password. The app and the database need the same values
so Nextcloud can connect to MariaDB. Using the same values in both places
keeps the setup consistent. It also makes the settings easy to change
without editing the images.

Deploying Nextcloud in a few minutes felt surprising. I wrote one file
and ran one command, and a working private cloud storage system was
running. I had a small problem when the terminal reconnected and Compose
could not find the file, but I fixed it by going back to the project
folder.

Since Mission 1, my understanding of cloud computing has grown. At first
I only knew basic ideas like storage and services. Now I know how to use
containers, work with data storage, and deploy a multi-container app. I
learned that cloud work is also about building and managing systems with
code, not just using them. This lab showed me that Infrastructure as Code
is a useful skill for a cloud engineer.
