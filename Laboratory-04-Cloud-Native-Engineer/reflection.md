# Mission Reflection

This laboratory activity helped me understand how containerization can simplify the deployment and management of applications. Compared with installing a complete operating system on a Virtual Machine, starting a Docker container is much faster because the container uses the existing host operating system kernel instead of requiring a separate guest operating system. In this activity, the Nginx server was downloaded and started with only a few Docker commands. This demonstrated how containers can provide a faster and more lightweight way to deploy suitable applications.

Port mapping is necessary because the web server inside the container is isolated from the host system. Nginx listens on port 80 inside the container, while the host uses port 8080 in this activity. The `-p 8080:80` option connects the host's port 8080 to port 80 inside the container, allowing users and applications on the host to access the Nginx web server through `http://localhost:8080`.

When the `docker rm` command is used, the specified container is removed from the Docker environment. Any data stored only inside the writable layer of that container is lost when the container is removed. Data that needs to survive the container lifecycle should instead be stored using Docker volumes or another persistent storage solution.

Containerization can also change how software developers and IT operations teams work together. Developers can package applications and their dependencies into consistent container images, while operations teams can deploy those same images across different environments. This supports a DevOps approach by reducing differences between development, testing, and production environments.

Finally, my GitHub portfolio is evolving from a collection of individual laboratory activities into a more organized record of my cloud computing skills. This laboratory added practical Docker and containerization experience to my previous cloud computing work. The screenshots, Markdown documentation, commands, and reflections provide evidence of both my technical work and my understanding of the concepts.
