1. Docker client is what you interact with, for example when you type "docker run nginx"
2. Docker Daemon is a background service that:
Builds images
Starts containers
Stops containers
Removes containers
Manages networks
Manages volumes
3. Docker Engine is the complete Docker platform.
It includes:
Docker Client
Docker Daemon
Docker API
Which makes Docker works
4. Docker registry stores Docker images. The most popular one is Docker Hub.
5. Difference between image and Container
Docker Image contains: Application code,
Libraries, Dependencies, Configuration.
Images are read-only.
You don't run an image directly.
While Docker Container is a running instance of an image.
6. Why containers are faster than virtual machines.

Containers run on the host machine's Linux kernel,  they are lightweight,  faster startup and use fewer resources while virtual machines have their operating systems, heavyweight,  slower startup and use more resources. 
