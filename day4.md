# Day 4 – Installing Docker on AWS EC2
 
## Overview
 
Successfully installed Docker on an Ubuntu 24.04 AWS EC2 instance and ran my first Docker container (`hello-world`). This was my first thorough practical experience using Docker on a cloud-hosted Linux server.
  
## 📌 What I Learned
 
 
- Updated and upgraded packages on an Ubuntu 24.04 EC2 instance.
 
- Installed Docker using the Ubuntu package manager.
 
- Learned how Docker downloads images from Docker Hub automatically when they are not available locally.
 
- Successfully ran the `hello-world` container to verify the Docker installation.
 
- Understood the relationship between the Docker Client, Docker Daemon, Docker Image, and Docker Container through a real-world example.
 

  
## ⚠️ Issues Encountered
 
### 1. SSH Authentication Failed
 
I initially received:
 
`Permission denied (publickey).`
 
This happened because I was using the wrong SSH command and PowerShell could not locate my private key (`.pem`) file.
 
### 2. Running Linux Commands in PowerShell
 
I attempted to run Linux commands such as:
 `sudo apt update ` 
inside Windows PowerShell, which resulted in command-not-found errors because I was not connected to the Ubuntu server.
 
### 3. Pending Kernel Upgrade
 
After upgrading the system, Ubuntu reported that a newer kernel had been installed and recommended rebooting the server to load the updated kernel.
  
## 🛠️ Resolution
 
 
- Located the correct private key (`vickykey1.pem`) and connected to the EC2 instance using the correct SSH command.
 
- Executed Linux commands only after successfully logging into the Ubuntu server.
 
- Rebooted the EC2 instance to load the updated Linux kernel.
 
- Verified that Docker was installed successfully by running:
 

 `sudo docker run hello-world ` 
The container downloaded successfully and displayed the **"Hello from Docker!"** message, confirming that Docker was working correctly.
  
## 📚 DevOps Lesson Learned
 
Docker images are downloaded only when they are not already available locally. The `docker run` command can automatically pull an image, create a container, and start it in a single command. Proper SSH configuration and understanding the difference between the local machine and a remote Linux server are essential skills for cloud engineers.
  
## 🚀 Summary
 
Successfully deployed Docker on an AWS EC2 Ubuntu server, resolved SSH and system update issues, and ran my first Docker container in the cloud. This marks the beginning of hands-on containerization in a real cloud environment.
