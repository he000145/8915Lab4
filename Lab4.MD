# CST8915 Lab 4: Docker

**Student Name**: Yiming He  
**Student ID**: 041-282-545  
**Course**: CST8915 Full-stack Cloud-native Development  
**Semester**: Winter 2026

---

## Demo Video

🎥 [Watch Demo Video](https://youtu.be/PLlaiaiA4HE)

---

## Reflection Questions

### What are the main differences between a Docker image and a Docker container?

A Docker container is a running instance of the image.

### Explain how Docker's layered architecture improves efficiency.

Docker image built with multiple read-only layers which are cached and shared across image. and all changes are make on the top writable layer. Then any across and rebuild will keep the same read-only layers and only work on new writable layer.

### Why does each container get its own writable layer?

Each container get its own writable layer will let any changes in one container won't effect other, they still keep the same read-only layers, it will support rollback or recreate anytime.

### What are the benefits of using Docker Compose over running containers individually?

Docker Compose make running multiple containers more easy. all made in one container's setting. It's easy to maintenance and monitor.