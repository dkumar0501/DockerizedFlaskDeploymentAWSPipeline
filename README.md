<h1 align="left">DockerizedFlaskDeploymentAWSPipeline</h1>

<p align="left">
  <strong>DevOps • Docker • Jenkins • AWS EC2 • CI/CD Automation</strong>
</p>

<!-- Badges -->
<p align="left">
  <img src="https://img.shields.io/badge/AWS-EC2%20Deployed-232F3E?logo=amazon-aws&logoColor=white" alt="AWS EC2">
  <img src="https://img.shields.io/badge/Docker-Containerized-blue?logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Jenkins-CI%2FCD%20Automated-red?logo=jenkins&logoColor=white" alt="Jenkins">
  <img src="https://img.shields.io/badge/Flask-Backend-lightgrey?logo=flask&logoColor=white" alt="Flask">
  <img src="https://img.shields.io/badge/MySQL-Database-4479A1?logo=mysql&logoColor=white" alt="MySQL">
</p>



### **About**
It is a **DevOps based automated deployment pipeline** that utilizes **Jenkins**, **Docker**, and **AWS EC2** to enable continuous integration and delivery of a two tier Flask MySQL web application, featuring **containerized services**, **GitHub integration**, and hands free application deployment through a fully automated **CI/CD workflow**.


## 📘 Overview

This project automates the deployment of a Flask application with a MySQL database on AWS EC2. It leverages **Jenkins pipelines**, **Docker Compose**, and **GitHub version control** to create a seamless DevOps workflow from code commit to production deployment ensuring reliability, scalability, and consistency.



## 🚀 Features

- Automated CI/CD pipeline with Jenkins  
- Dockerized two tier Flask MySQL application  
- Continuous integration via GitHub webhooks  
- One click container orchestration with Docker Compose  
- AWS EC2 based production environment  
- Streamlined and hands free deployment process  



## 🧠 Technical Overview

| Component | Description |
|------------|-------------|
| **Infrastructure** | AWS EC2 (Ubuntu 22.04 LTS) |
| **Backend Framework** | Flask (Python 3.9) |
| **Database** | MySQL (containerized with persistent storage) |
| **Containerization** | Docker & Docker Compose |
| **CI/CD Tool** | Jenkins (Pipeline-as-Code via Jenkinsfile) |
| **Version Control** | GitHub integration with Jenkins |
| **Automation Flow** | Code push → Jenkins build → Docker image → Docker Compose deploy |



## ⚙️ Architecture Overview

```
+-----------------+      +----------------------+      +-----------------------------+
|   Developer     |----->|     GitHub Repo      |----->|        Jenkins Server       |
| (pushes code)   |      | (Source Code Mgmt)   |      |  (on AWS EC2)               |
+-----------------+      +----------------------+      |                             |
                                                       | 1. Clones Repo              |
                                                       | 2. Builds Docker Image      |
                                                       | 3. Runs Docker Compose      |
                                                       +--------------+--------------+
                                                                      |
                                                                      | Deploys
                                                                      v
                                                       +-----------------------------+
                                                       |      Application Server     |
                                                       |      (Same AWS EC2)         |
                                                       |                             |
                                                       | +-------------------------+ |
                                                       | | Docker Container: Flask | |
                                                       | +-------------------------+ |
                                                       |              |              |
                                                       |              v              |
                                                       | +-------------------------+ |
                                                       | | Docker Container: MySQL | |
                                                       | +-------------------------+ |
                                                       +-----------------------------+
```


## 🧩 Future Enhancements

- Integration with **Kubernetes** for scalable orchestration  
- Monitoring and alerting with **Prometheus & Grafana**  
- Secure **secrets management** using AWS Secrets Manager  
- Implementation of **Blue-Green / Canary** deployment strategy  
- Automated rollback for failed builds  



## 👨‍💻 Author

**Developed by [D Kumar](https://github.com/dkumar0501)** **[IIT Patna]**


<p align="center">
  <em>“Bridging development and deployment through intelligent automation.”</em>
</p>
