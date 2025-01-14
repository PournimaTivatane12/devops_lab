# Prerequisites for CI/CD Pipeline Setup with Jenkins and Docker

## Author: Pournima Tivatane

This document outlines the prerequisites needed to set up and deploy a CI/CD pipeline using Jenkins and Docker.

---

## System Requirements

1. **Operating System**: Linux (Ubuntu 20.04+ recommended) or Windows 10/11 with WSL.
2. **Hardware Requirements**:
   - Minimum 4 GB RAM (8 GB recommended for smoother operation).
   - At least 20 GB free disk space.
   - A stable internet connection.

---

## Software Requirements

1. **JDK**:
   - Jenkins requires Java Development Kit (JDK) version 11 or later.
   - Verify Java installation:
     ```bash
     java -version
     ```
2. **Jenkins**:
   - Install Jenkins on the host machine. Follow the official Jenkins installation guide: [Jenkins Installation](https://www.jenkins.io/doc/book/installing/).

3. **Docker**:
   - Install Docker on the host machine. Follow the official Docker installation guide: [Docker Installation](https://docs.docker.com/get-docker/).
   - Verify Docker installation:
     ```bash
     docker --version
     ```

4. **Git**:
   - Ensure Git is installed for version control.
   - Verify Git installation:
     ```bash
     git --version
     ```

5. **Docker Compose** (Optional):
   - Required if using `docker-compose` to manage multi-container setups.
   - Verify Docker Compose installation:
     ```bash
     docker-compose --version
     ```

---

## Networking Requirements

1. **Ports**:
   - Jenkins: `8080` (default, ensure it's open).
   - Docker daemon: Ensure access to required ports for container networking.
2. **Firewall Rules**:
   - Allow inbound traffic on the necessary ports.
   - Example command for UFW on Ubuntu:
     ```bash
     sudo ufw allow 8080
     ```

---

## Access and Permissions

1. **User Permissions**:
   - Ensure the user running Jenkins has `sudo` access for administrative tasks.
   - Add the Jenkins user to the `docker` group:
     ```bash
     sudo usermod -aG docker jenkins
     ```

2. **Repository Access**:
   - Clone or pull the source code from the Git repository. Ensure SSH or HTTPS access is configured.

---

## Environment Variables

Prepare the following environment variables:
- `DOCKER_USERNAME`: Docker Hub username.
- `DOCKER_PASSWORD`: Docker Hub password or access token.
- `REPO_URL`: URL of the source code repository.

---

## Additional Requirements

1. **Pipeline Configuration**:
   - Ensure a `Jenkinsfile` is present in the source code repository for pipeline definition.
2. **Dockerfile**:
   - A valid `Dockerfile` must exist in the project root directory for image building.

---

## References

- [Jenkins Official Documentation](https://www.jenkins.io/doc/)
- [Docker Official Documentation](https://docs.docker.com/)
- [Git Official Documentation](https://git-scm.com/doc)
