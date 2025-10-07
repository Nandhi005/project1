# Project1 – DevOps Workflow on AWS EC2

This project demonstrates a complete **DevOps pipeline** hosted on **AWS EC2**, integrating **Jenkins, Docker (Tomcat), Ansible, and Git** to automate web application deployment.

---

## 🚀 Project Overview

The goal of this project is to showcase:

- Continuous Integration and Deployment using **Jenkins**
- Containerization using **Docker with Tomcat**
- Configuration management using **Ansible**
- Version control using **Git**
- Hosting and running services on **AWS EC2**
- Automating deployment using **Publish Over SSH** and **Remote Exec** in Jenkins

This setup provides a real-world workflow for deploying Java web applications in a scalable and automated manner.

---

## 🛠️ Technologies Used

- **AWS EC2** – Virtual servers to host Jenkins and Docker containers  
- **Jenkins** – CI/CD automation server  
- **Docker (Tomcat)** – Containerization for Java web applications  
- **Ansible** – Configuration management and deployment automation  
- **Git** – Version control for source code  
- **Jenkins Plugins**:  
  - **Poll SCM** – Automatically detects Git changes  
  - **Publish Over SSH** – Sends files and commands to remote servers  
  - **Remote Exec** – Executes commands on remote servers  

---

## 📌 Architecture

1. **Git**: Stores and versions the web application code.  
2. **Jenkins**: Polls SCM for changes, builds Docker images, and triggers deployment.  
3. **Publish Over SSH & Remote Exec**: Deploys Docker container to the remote EC2 server.  
4. **Docker (Tomcat)**: Runs the web application in containers, deploying directly to `/usr/local/tomcat/webapps`.  
5. **Ansible**: Optionally automates server setup and deployment.  
6. **AWS EC2**: Hosts Jenkins server and runs Docker containers.  

---

## 💻 Getting Started

### Prerequisites

- AWS account with EC2 instance access  
- Jenkins installed on EC2 (or local)  
- Docker installed on EC2  
- Ansible installed on local machine (optional)  
- Git installed locally  
- SSH access to EC2 server  

---

### Steps to Run

#### 1. Clone the repository

```bash
git clone https://github.com/Nandhi005/project1.git
cd project1

