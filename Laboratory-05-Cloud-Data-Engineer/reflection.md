# Mission Reflection

Object storage works better for millions of photos than block storage because it doesn't 
use a normal folder system. Each photo is just saved as an object with an ID and some 
metadata, so it's easy to spread across many servers as things grow. Block storage is 
made for fast access to structured data like databases, not for storing tons of random 
files.

Docker made deploying MinIO a lot easier. I didn't have to install anything manually — one 
docker run command with the right flags set up the server, the login, and the ports all 
at once. This actually helped a lot when I hit a problem: the official minio/minio image 
was taken down from Docker Hub, so I had to switch to a different image (tobi312/minio) 
instead. Since Docker containers work the same way no matter which image you use, swapping 
it out was quick and didn't break anything else in the setup.

A "bucket" is basically just a storage container for objects. It's like a top-level folder, 
but without the usual nested folder structure you'd see in a normal file system.

For big companies, I think they avoid losing data by copying it across multiple servers or 
even different locations, so if one server goes down, the data is still safe somewhere 
else. They probably also use some kind of automatic backup or replication system running 
in the background all the time.

My confidence with the Linux command line is getting better. Running into the Docker image 
issue and having to figure it out on my own — reading the error, searching for a fix, and 
trying a different image — helped more than just following the steps exactly as written. 
It made me actually think about what each command was doing instead of just copy-pasting.
