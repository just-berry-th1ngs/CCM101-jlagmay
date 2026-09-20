# Lab 04 Reflection

1. **Container vs. VM setup.** Running Nginx took three commands: pull, run, and curl. The web server was up in seconds. A VM needs a full operating system installed first, which means an installer, setup steps, and a long boot each time. A container skips all of that because it shares the host's OS and only starts the app.

2. **Why port mapping is needed.** A container is isolated, so nothing outside it can reach the ports inside by default. Nginx listens on port 80 inside the container, but my machine cannot see that port. The flag `-p 8080:80` connects port 8080 on my machine to port 80 in the container. That is why `curl http://localhost:8080` worked.

3. **What `docker rm` does to data.** While a container runs, its data is kept in a writable layer that belongs to that container. When I ran `docker rm my-nginx`, that layer was deleted, so anything saved only inside the container is lost. Data can outlive a container if it is stored in a volume or a bind mount, because those live outside the container. For data that matters, such as a database, I should use a volume.

4. **Effect on DevOps teamwork.** "It works on my machine" happens when developers and IT have different setups. A container image packages the app with everything it needs, so both teams run the same thing in development, testing, and production. Developers hand over an image instead of setup notes, and IT can deploy it without guessing what is missing. This means fewer setup problems and fewer arguments about whose setup is wrong.

5. **My GitHub portfolio.** Since Lab 1, my portfolio has become more organized. Each lab has its own folder, and Lab 4 has a README, documentation files, and screenshots as proof of my work. Someone can open the README and understand the lab in a minute. I also now write down each command with a short note on what it does, which helps me review later.

*AI disclosure: Claude helped with the wording of this reflection.*
