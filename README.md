**Project Overview**
This project **TriLayer WebOps: Dockerized & Kubernetes Orchestrated** demonstrates the deployment of a three-tier web application using Docker and Kubernetes. It includes configuration management with Ansible, application code management with Git, a CI/CD pipeline for application deployment using Jenkins, and application monitoring via AWS-Cloudwatch.

Technologies Used
**Docker:** Containerization of the application components.
**Kubernetes:** Orchestrating the deployment, scaling, and management of containerized applications.
**Ansible:** Configuration management and automation using Ansible roles.
**Git:** Version control for application code and configuration files.
**Jenkins:** Continuous Integration and Continuous Deployment (CI/CD) pipeline.
**Monitoring Tools:** Tools for monitoring application performance and health.

**Project Components**
a. TriLayer WebOps: Dockerized & Kubernetes Orchestrated
The application is divided into three tiers:

Frontend: The user interface of the application.
Backend: The server-side logic and operations.
Database: The storage for application data.
These components are containerized using Docker and managed with Kubernetes for orchestration.

b. Configuration Management Using Ansible (Roles)
Ansible is used to automate the configuration and setup of the environment. The following Ansible playbook and roles are used:

ansible.yml: Main playbook that includes the necessary roles and tasks.
roles/: Directory containing Ansible roles for different components.
c. Application Code Management Using Git
The application code and configuration files are managed using Git. This allows for version control and collaboration.

d. Building CI/CD Pipeline to Deploy a New Version of Application (Jenkins)
Jenkins is used to set up a CI/CD pipeline that automates the build, test, and deployment process. This ensures that new versions of the application are deployed efficiently and consistently.

e. Building Monitoring for Application
Monitoring tools are integrated to track the application's performance, availability, and health. This helps in proactive identification and resolution of issues.

**File Structure**


project-root/
├── ansible/
│   ├── ansible.yml
│   └── roles/
│       ├── role1/
│       │   └── tasks/
│       │       └── main.yml
│       ├── role2/
│       │   └── tasks/
│       │       └── main.yml
│       └── ...
├── kubernetes/
│   ├── deployment.yml
│   └── service.yml
├── docker/
│   └── Dockerfile
├── jenkins/
│   └── Jenkinsfile
├── monitoring/
│   └── monitoring-setup.yml
└── README.md



**Key Files**
ansible.yml: Main Ansible playbook.
deployment.yml: Kubernetes deployment configuration.
service.yml: Kubernetes service configuration.
Dockerfile: Dockerfile for building the application image.
Jenkinsfile: Jenkins pipeline configuration.
monitoring-setup.yml: Configuration for setting up application monitoring.

**How to Use**
**Clone the Repository:**
git clone https://github.com/ankurbhardwajkiet/three-tier-web-app.git
cd three-tier-web-app

**Set Up Environment:
Use Ansible to set up the environment:**
ansible-playbook ansible/ansible.yml

**Build and Deploy with Docker and Kubernetes:**
kubectl apply -f kubernetes/deployment.yml
kubectl apply -f kubernetes/service.yml

**Configure CI/CD Pipeline:**
Set up Jenkins and use the provided Jenkinsfile to configure the CI/CD pipeline.

**Monitor the Application:**
Use the monitoring tools configured in monitoring/monitoring-setup.yml.

