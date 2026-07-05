🐳 Day 6 – Docker Container Lifecycle
📌 Overview
In Day 6, I learned how to manage the lifecycle of Docker containers and understand how containers behave from creation to deletion. This included working with running, stopped, and removed containers, and understanding how Docker manages state.
📚 What I Learned
Understood the full Docker container lifecycle:
Create
Start
Stop
Restart
Remove
Learned the difference between:
docker run (creates and starts a new container)
docker start (starts an existing container)
Understood that containers are lightweight and temporary by design.
Practiced controlling container states using Docker commands.
Learned that images remain unchanged even when containers are stopped or removed.
⚠️ Challenges Encountered
Initially confused docker run and docker start as doing the same thing.
Needed clarification on how containers differ from images in terms of lifecycle and persistence.
🛠️ Resolution
Practiced both commands hands-on using real containers.
Observed that:
docker run creates a new container each time
docker start only resumes an existing stopped container
This clarified the difference between creation and reusability of containers.
📌 DevOps Lesson Learned
Docker containers are ephemeral by design, meaning they can be created, stopped, restarted, and removed easily without affecting the image. Understanding container state management is essential for running and maintaining applications in production environments.
🚀 Summary
Successfully learned and practiced Docker container lifecycle management, gaining a clear understanding of how containers move between different states and how Docker manages them internally.
