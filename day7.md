# 🐳 Day 7 – Docker Images Deep Dive

## 📌 Overview

In Day 7, I learned what Docker images are made of, how they work internally, and why they are efficient. I explored how images are structured in layers, how Docker reuses cached layers, and how tagging helps manage different versions of images.

---

## 📚 What I Learned

- Docker images are **read-only templates** used to create containers.
- Images are built in **layers**, and each instruction in a Dockerfile creates a new layer.
- Docker uses **layer caching** to speed up builds and reduce resource usage.
- Learned the difference between:
  - `docker pull` → downloads an image from Docker Hub
  - `docker run` → creates and starts a container from an image
- Understood image tagging:
  - `latest` tag
  - version-specific tags (e.g. `nginx:1.25`)
- Learned that multiple containers can be created from a single image.

---

## ⚠️ Challenges Encountered

- Initially confused how Docker images are reused efficiently for multiple containers.
- Needed clarity on why Docker does not re-download images every time.
- Understanding image layers and caching required hands-on practice.

---

## 🛠️ Resolution

- Practiced pulling and running images multiple times to observe caching behavior.
- Learned that Docker stores image layers locally for efficiency.
- Understood that containers are created independently from images without modifying the original image.
- Observed how image tags determine which version of an image is used.

---

## 📌 DevOps Lesson Learned

Docker images use a layered architecture that makes them lightweight, reusable, and efficient. Understanding image layers and caching is essential for optimizing builds and managing containerized applications effectively.

---

## 🚀 Summary

Successfully understood Docker images in depth, including layers, caching, tagging, and image reuse. This knowledge improves efficiency when building and deploying containerized applications.
