🐳 Day 8 – Dockerfile Basics & Building Your Own Image
📌 Overview
In Day 8, I learned how to create a Dockerfile and build my own custom Docker image. This helped me understand how applications are packaged into images and how Docker automates environment setup using instructions written in a Dockerfile.
📚 What I Learned
A Dockerfile is a script used to build Docker images automatically.
It contains step-by-step instructions for creating an image.
Learned common Dockerfile instructions:
FROM → base image
RUN → executes commands during build
COPY → copies files into the image
WORKDIR → sets working directory
CMD → default command when container starts
Learned how to build images using:
docker build -t image-name .
Learned how to run custom-built images using docker run.
⚠️ Challenges Encountered
Initially struggled to understand the difference between a Dockerfile and an image.
Had to carefully follow syntax rules (small mistakes in Dockerfile can break builds).
Understanding the order of instructions in Dockerfile was important.
🛠️ Resolution
Practiced writing a simple Dockerfile step-by-step.
Built and tested images multiple times to understand build output.
Learned that Docker builds images layer by layer based on Dockerfile instructions.
Understood that correcting Dockerfile order improves build efficiency.
📌 DevOps Lesson Learned
Dockerfiles allow automation of environment setup, making applications portable and reproducible. Instead of manually configuring systems, we define everything in code and let Docker build consistent environments across different machines.
🚀 Summary
Successfully learned how to create a Dockerfile and build a custom Docker image. This is a major step toward real-world DevOps workflows where infrastructure and applications are defined as code.
