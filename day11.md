🚀 Now: Day 11 – Docker Compose (Overview)
📌 Overview
In Day 11, I learned about Docker Compose and how it is used to manage multiple containers at once using a single configuration file. I understood how Docker Compose simplifies running complex applications that require more than one service.
📚 What I Learned
Docker Compose is used for multi-container applications
Instead of running multiple docker run commands, we use a single YAML file
Services are defined in docker-compose.yml
One command can start everything:
docker-compose up -d
One command can stop everything:
docker-compose down
🧠 Key Concepts
Service → Each container in Compose
YAML file → Configuration file (docker-compose.yml)
Orchestration → Managing multiple containers together
⚙️ Example Structure
version: '3'
services:
  web:
    image: nginx
    ports:
      - "80:80"
  app:
    image: node
🚨 Challenges Encountered
Confusion between Docker CLI and Docker Compose
Understanding YAML syntax
Learning how multiple services interact
🛠️ How I Resolved It
Learned that Compose replaces multiple docker run commands
Understood structure of YAML files
Practiced defining services and ports
Realized Compose is used in real production environments
🎯 Final Result
Successfully understood Docker Compose and how it simplifies multi-container deployments.
💡 Key Lesson
Instead of managing containers one by one, Docker Compose allows you to manage an entire application stack with one file and one command.
🚀 DevOps Insight
Real-world applications often include:
Web server (Nginx)
Backend API (Node/Python)
Database (MySQL/PostgreSQL)
Docker Compose manages all of them together.
