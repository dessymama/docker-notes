🐳 Day 12 – Docker Compose Hands-on Project
📌 Overview
In Day 12, I practiced Docker Compose by building a simple multi-container application. I learned how Docker Compose is used to manage multiple containers as a single application using a docker-compose.yml file.
📚 What I Learned
Docker Compose is used for multi-container applications
It replaces multiple docker run commands with one configuration file
All services are defined inside a docker-compose.yml file
One command can start the entire application stack:
docker-compose up -d
One command can stop everything:
docker-compose down
⚙️ Practical Understanding
Example docker-compose.yml
version: "3"

services:
  web:
    image: nginx
    ports:
      - "80:80"

  app:
    image: node
    command: node server.js
🚨 Challenges Encountered
Confusion between Docker CLI and Docker Compose
YAML indentation issues
Errors due to incorrect service definitions
Understanding how multiple containers work together
🛠️ How I Resolved It
Learned correct YAML formatting rules
Understood that Compose manages full application stacks
Practiced starting and stopping multiple services together
Used docker ps and logs to debug issues
🎯 Final Result
Successfully built and managed a multi-container application using Docker Compose.
💡 Key Lesson
Docker Compose simplifies complex applications by allowing multiple containers to be managed using a single file and one command.
🚀 DevOps Insight
In real-world systems:
Frontend runs in one container (e.g., Nginx)
Backend runs in another (Node/Python)
Database runs separately (MySQL/PostgreSQL)
Docker Compose brings all of them together for easy development and deployment.
