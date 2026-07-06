🐳 Day 20 – Docker Mini Project (Portfolio Project)
📌 IMPORTANT (Before Hands-on)

📌 Overview
I combined the Docker concepts I learned throughout the course into a small portfolio project. I reviewed images, containers, networking, volumes, Docker Compose, Docker Hub, and production concepts to understand how they work together in a real deployment.
📚 Skills Applied
Running Docker containers
Port mapping
Docker networking
Docker volumes
Docker Compose
Building Docker images with a Dockerfile
Docker Hub concepts
Container debugging
Restart policies
🏗️ Mini Project Architecture
Browser
   │
   ▼
EC2 Instance
   │
   ▼
Docker Engine
   │
   ▼
Nginx Container
This simple project demonstrates deploying a containerized web server on AWS.
⚙️ Commands Reviewed
Pull an image
docker pull nginx
Run Nginx
docker run -d --name web1 -p 80:80 nginx
Check running containers
docker ps
View logs
docker logs web1
Stop a container
docker stop web1
Remove a container
docker rm web1
🚨 Challenges Encountered
Public IP changed after restarting EC2
Docker permission issues
Container name conflicts
Browser could not initially reach Nginx
Understanding Docker networking and port mapping
🛠️ How I Resolved Them
Updated SSH command with the new EC2 public IP
Used sudo or proper Docker permissions
Removed or renamed conflicting containers
Verified Security Group inbound rules
Confirmed port mapping with docker ps
Tested locally using curl localhost
🎯 Final Result
Successfully deployed and managed Docker containers on an AWS EC2 Ubuntu server, gaining hands-on experience with the complete Docker workflow.
💡 Key Lesson
Docker is more than running containers—it provides a complete platform for packaging, deploying, managing, and troubleshooting applications consistently across environments.
