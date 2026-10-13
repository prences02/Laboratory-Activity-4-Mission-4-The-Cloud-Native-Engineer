# Laboratory 04 Reflection

This laboratory helped me  to understand the importance of Docker and containerization in cloud computing. I learned that containers provide a faster and more efficient way to deploy an applications compared to traditional virtual machines.

First, Docker containers usually start in seconds because they share the host operating system kernel. In contrast, virtual machines need to start their own guest operating systems, which requires more time and resources. With Docker, developers can package an application and its dependencies into a container instead of installing an entire operating system for every application.

Second, port mapping is necessary because it allows users to access a service running inside a container through a port on the host machine. In my activity, I used `-p 8080:80` to connect host port 8080 to port 80 inside the Nginx container.

Third, the `docker rm` command removes a stopped container. Data stored only in the container's writable layer is removed with the container. However, data stored in persistent volumes can remain available even after the container is deleted. This taught me why persistent storage is important when applications need to keep their data.

Fourth,  The containerization improves collaboration between software developers and IT operations teams. Developers can package applications in consistent environments, while the operations teams can deploy and manage those applications more easily. This supports DevOps practices by improving consistency, automation, and communication.


