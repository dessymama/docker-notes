🐳 Day 17 – Docker Image Building (Routine Overview)
📌 IMPORTANT (Before Hands-on)
👉 START EC2 INSTANCE before doing practical work
📌 Overview
In Day 17, I learned how to build custom Docker images using a Dockerfile. Instead of using pre-built images, I learned how to package my own application into a Docker image.
📚 What I Learned
A Dockerfile is used to create custom Docker images
Images are built in layers
Each instruction creates a new image layer
docker build is used to create images
Custom images allow you to containerize your own applications
🧱 Key Dockerfile Instructions
FROM → base image
WORKDIR → sets working directory
COPY → copies files into the image
RUN → executes commands during build
CMD → default command when container starts
⚙️ Example Dockerfile
FROM nginx

WORKDIR /usr/share/nginx/html

COPY . /usr/share/nginx/html

CMD ["nginx", "-g", "daemon off;"]
🚀 Commands Practiced
Build Docker image
docker build -t my-nginx-app .
List Docker images
docker images
Run container from image
docker run -d -p 80:80 my-nginx-app
🚨 Challenges Encountered
Confusion about Dockerfile syntax and structure
Understanding how image layers are created
Errors due to incorrect file paths
Forgetting to rebuild image after updates
🛠️ How I Resolved It
Learned correct Dockerfile structure
Understood step-by-step image building process
Rebuilt images after every change
Used logs and container inspection for debugging
🎯 Final Result
Successfully built and ran a custom Docker image using a Dockerfile.
💡 Key Lesson
Docker allows you to build your own images, not just use existing ones — this is how real applications are packaged.
🚀 DevOps Insight
In real-world DevOps:
Developers write Dockerfiles for applications
CI/CD pipelines automatically build images
Images are stored in Docker Hub or AWS ECR
Containers are deployed from custom images

