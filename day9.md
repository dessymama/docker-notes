🐳 Day 9 – Docker Networking (Overview)
📌 What I Learned
In Day 9, I learned about Docker networking and how containers communicate with the outside world using port mapping. I understood that each container is isolated and requires proper network configuration to be accessible externally.
🌐 Key Concepts
Docker containers are isolated by default
Networking allows containers to communicate externally
Default Docker network is bridge network
Port mapping connects EC2 ports to container ports
Example: -p 80:80 maps EC2 port 80 to container port 80
🧠 Important Commands Practiced
docker run -d -p 80:80 nginx
docker ps
curl localhost
docker stop <container_id>
docker rm <container_id>
🚨 Challenges Encountered
Browser could not access Nginx container initially
EC2 public IP changed after restart
Container created without proper port exposure
Confusion with existing stopped containers
Container name conflict when trying to reuse web1
🛠️ How I Resolved It
Checked running and stopped containers using docker ps -a
Removed conflicting container using docker rm
Restarted container with correct port mapping (-p 80:80)
Verified EC2 Security Group allowed port 80
Confirmed EC2 public IP was correct
Successfully accessed Nginx in browser
🎯 Final Result
Successfully deployed an Nginx container on EC2 and accessed it through the browser using public IP. The setup confirmed understanding of Docker networking and port mapping.
💡 Key Lesson
Docker containers are isolated by default. To make them accessible externally, you must explicitly expose ports using -p hostPort:containerPort and ensure AWS Security Groups allow traffic.
🚀 DevOps Insight
Real-world deployments require:
Proper networking setup
Firewall configuration (AWS Security Groups)
Correct container port mapping
Debugging skills when services are not reachable
