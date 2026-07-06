🐳 Day 18 – Docker Registry (Docker Hub Deep Dive)

📌 Overview
In Day 18, I learned about Docker Registry and how Docker images are stored, shared, and managed using Docker Hub. I understood how to push custom images and pull them from remote repositories.
📚 What I Learned
A Docker Registry stores Docker images
Docker Hub is the most popular public registry
You can push and pull images from Docker Hub
Images must be properly tagged before pushing
Registries are essential for CI/CD pipelines
🌐 Key Concepts
docker pull → download image from registry
docker push → upload image to registry
docker login → authenticate Docker Hub
docker tag → rename image for registry upload
⚙️ Commands Practiced
Login to Docker Hub
docker login
Tag an image
docker tag my-nginx-app username/my-nginx-app:v1
Push image
docker push username/my-nginx-app:v1
Pull image
docker pull username/my-nginx-app:v1
🚨 Challenges Encountered
Confusion with image tagging format
Authentication issues with Docker Hub
Errors when pushing untagged images
Understanding repository naming rules
🛠️ How I Resolved It
Learned correct format: username/image:tag
Used docker login for authentication
Tagged images before pushing
Verified images on Docker Hub website
🎯 Final Result
Successfully learned how to store and share Docker images using Docker Hub registry.
💡 Key Lesson
Docker Registry is where container images live — enabling sharing, versioning, and deployment across different environments.
