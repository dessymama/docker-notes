Day 5- Running Your First Web Server in Docker


Overview
Deploying Nginx inside a Docker container and accessing it through your EC2 public IP.

What I learned.
1. How to pull an image manually.
2. How to start a container.
3. How to view running containers.
4. How Docker exposes ports.
5. How to stop and remove containers.
6. How to verify a container is serving traffic.


Issue encountered 
No issue encountered because every command was carefully selected. 

DevOps Lesson Learned 
If everything is configured correctly,  I should see the "Welcome to nginx" page

Summary 
Everything worked well, from pulling the nginx image to running it in the background,  mapping port 80 on my EC2 instance to port 80 inside the container to giving it a friendly name . Also verify it's running,  tested it on my browser ( i saw the"Welcome to nginx" page). I stopped and removed the container when I was done.
