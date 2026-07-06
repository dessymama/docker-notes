🐳 Day 17 – Docker Image Building (Dockerfile Deep Dive)

📌 Overview
In Day 17, I learned how to build custom Docker images using a Dockerfile. Instead of using pre-built images, I learned how to package my own application into a Docker image that can be run as a container.
📚 What I Learned
A Dockerfile is used to create custom Docker images
Images are built in layers
Each instruction in a Dockerfile creates a new layer
docker build is used to create images
Custom images allow applications to be containerized
🧱 Key Dockerfile Instructions
FROM → base image
WORKDIR → sets working directory inside container
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
Confusion about Dockerfile syntax
Understanding image layering process
Errors due to incorrect file paths
Forgetting to rebuild after changes
🛠️ How I Resolved It
Learned correct Dockerfile structure
Understood step-by-step build process
Rebuilt images after every change
Used logs and container inspection for debugging
🎯 Final Result
Successfully built and ran a custom Docker image using a Dockerfile.
💡 Key Lesson
Docker allows you to build your own images — not just use existing ones — which is how real applications are packaged.
🚀 DevOps Insight
In real-world DevOps:
Developers write Dockerfiles for applications
CI/CD pipelines automatically build images
Images are pushed to Docker Hub or AWS ECR
Containers are deployed from these custom images
