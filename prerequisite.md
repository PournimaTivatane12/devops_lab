# Prerequisites for DevOps Lab

Welcome to the DevOps Lab repository! Before you begin working with this project, please ensure that you have the following prerequisites in place. These tools and configurations will help you set up your environment seamlessly.

---

## 1. System Requirements
- **Operating System**: Linux, macOS, or Windows (WSL recommended for Windows users)
- **Processor**: Dual-core or higher
- **RAM**: At least 4 GB (8 GB or more recommended for running multiple tools simultaneously)
- **Disk Space**: At least 10 GB free space

---

## 2. Software and Tools
Ensure the following software is installed on your system:

### Development Tools
- **Git**: Version control system for cloning and managing the repository.
  - Installation Guide: [Git Documentation](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- **Docker**: To build and manage containerized applications.
  - Installation Guide: [Docker Documentation](https://docs.docker.com/get-docker/)
- **Kubernetes CLI (kubectl)**: To interact with Kubernetes clusters.
  - Installation Guide: [Kubernetes Documentation](https://kubernetes.io/docs/tasks/tools/)
- **Terraform**: For infrastructure as code (IaC).
  - Installation Guide: [Terraform Documentation](https://developer.hashicorp.com/terraform/tutorials)
- **AWS CLI**: For managing AWS resources from the command line.
  - Installation Guide: [AWS CLI Documentation](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)

---

## 3. Cloud Account
You need access to a cloud platform (AWS recommended) with the following:
- **AWS Account**: [Sign up here](https://aws.amazon.com/)
- IAM role with the necessary permissions to:
  - Create and manage EC2 instances
  - Use S3 buckets
  - Configure IAM roles and policies

---

## 4. Programming Languages
- **Python 3.8+**: For scripting and automation tasks.
  - Installation Guide: [Python Documentation](https://www.python.org/downloads/)
- **Node.js (Optional)**: If the project involves JavaScript-based tools or frameworks.
  - Installation Guide: [Node.js Downloads](https://nodejs.org/)

---

## 5. Integrated Development Environment (IDE)
Use a code editor or IDE of your choice. Recommended:
- **Visual Studio Code**
  - Extensions:
    - Docker
    - Kubernetes
    - Terraform
    - Python

---

## 6. Networking
- Ensure that the following ports are open in your local firewall:
  - **22**: For SSH connections
  - **80/443**: For web applications
  - **6443**: For Kubernetes API server access (if running a local cluster)

---

## 7. Knowledge Prerequisites
- Basic understanding of:
  - Linux commands
  - Version control using Git
  - Containers and container orchestration (e.g., Docker and Kubernetes)
  - Infrastructure as Code (Terraform or similar tools)
  - AWS services (EC2, S3, IAM, etc.)

---

## 8. Optional Tools
For easier management and debugging:
- **Helm**: Kubernetes package manager
  - Installation Guide: [Helm Documentation](https://helm.sh/docs/intro/install/)
- **Postman**: For testing APIs
  - Installation Guide: [Postman Downloads](https://www.postman.com/downloads/)
- **tmux**: For managing multiple terminal sessions
  - Installation Guide: [tmux Documentation](https://github.com/tmux/tmux)

---

## 9. Clone the Repository
Once the above prerequisites are met, clone this repository to your local machine:
```bash
git clone https://github.com/PournimaTivatane12/devops_lab.git
cd devops_lab
