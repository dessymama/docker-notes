🐳 Day 19 – Docker Production Concepts (Restart Policies & Health Checks)

📌 Overview
In Day 19, I learned about Docker production-level concepts such as restart policies and health checks. I understood how containers behave in real production environments and how Docker ensures application reliability.
📚 What I Learned
Containers can fail or stop unexpectedly
Docker provides restart policies to auto-recover containers
Health checks are used to monitor container status
These features are important in production systems
Helps ensure high availability of applications
🔁 Restart Policies
Types of restart policies:
no → default, do not restart
always → always restart container
on-failure → restart only if container fails
unless-stopped → restart unless manually stopped
Example:
docker run -d --restart always nginx
❤️ Health Checks (Concept)
Health checks monitor if a container is working properly.
Example (Dockerfile concept):
HEALTHCHECK CMD curl --fail http://localhost || exit 1
⚙️ Commands Practiced
Run container with restart policy
docker run -d --restart unless-stopped nginx
Check running containers
docker ps
Inspect container
docker inspect <container_id>
🚨 Challenges Encountered
Confusion about when containers restart
Understanding difference between manual stop and crash
Difficulty understanding health check behavior
Not knowing real production usage
🛠️ How I Resolved It
Tested container restart behavior manually
Learned difference between policies
Understood that Docker manages recovery automatically
Studied how health checks monitor container status
🎯 Final Result
Successfully learned how Docker ensures container reliability using restart policies and health checks.
💡 Key Lesson
In production, containers must be self-healing — Docker restart policies and health checks help achieve that.
