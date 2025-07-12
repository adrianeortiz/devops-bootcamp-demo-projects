# DevOps Bootcamp Demo Projects

This repository contains 58 scaffolded demo projects covering various DevOps technologies and practices. Each project is a complete Git repository with starter code, configuration files, and CI/CD pipelines.

## 📚 Module Overview

### Module 5: Cloud & Infrastructure as Service Basics
- **create-server-and-deploy-application-on-digitalocean** - Setup and configure a server on DigitalOcean, create Linux user, deploy Java Gradle application
- **run-nexus-on-droplet-and-publish-artifact-to-nexus** - Install and configure Nexus from scratch, create users with permissions, build and upload JAR files

### Module 6: Artifact Repository Manager with Nexus
- **run-nexus-on-droplet-and-publish-artifact-to-nexus** - Install and configure Nexus from scratch, create users with permissions, build and upload JAR files

### Module 7: Containers with Docker
- **use-docker-for-local-development** - Create Dockerfile for Node.js application, run in Docker container with MongoDB and MongoExpress
- **docker-compose-run-multiple-docker-containers** - Write Docker Compose file to run MongoDB and MongoExpress containers
- **deploy-docker-application-on-a-server-with-docker-compose** - Copy Docker-compose file to remote server, login to private registry, start application
- **dockerize-nodejs-application-and-push-to-private-docker-registry** - Write Dockerfile, create private Docker registry on AWS (Amazon ECR), push image
- **create-docker-repository-on-nexus-and-push-to-it** - Create Docker hosted repository on Nexus, configure permissions, build and push Docker image
- **persist-data-with-docker-volumes** - Persist data of MongoDB container by attaching Docker volume
- **deploy-nexus-as-docker-container** - Create and configure Droplet, set up and run Nexus as Docker container

### Module 8: Build Automation & CI/CD with Jenkins
- **install-jenkins-on-digitalocean** - Create Ubuntu server on DigitalOcean, set up and run Jenkins as Docker container, initialize Jenkins
- **create-a-ci-pipeline-with-jenkinsfile-freestyle-pipeline-multibranch-pipeline** - CI Pipeline for Java Maven application, install build tools, create different Jenkins job types
- **create-a-jenkins-shared-library** - Create Jenkins Shared Library to extract common build logic, create functions, integrate in Jenkins Pipeline
- **configure-webhook-to-trigger-ci-pipeline-automatically-on-every-change** - Install GitLab Plugin, configure GitLab access token, configure Jenkins to trigger CI pipeline
- **dynamically-increment-application-version-in-jenkins-pipeline** - Configure CI steps for version increment, build application, build Docker image, push to repository

### Module 9: AWS Services
- **deploy-web-application-on-ec2-instance-manually** - Create and configure EC2 Instance on AWS, install Docker, deploy Docker image
- **cd-deploy-application-from-jenkins-pipeline-to-ec2-instance-automatically-with-docker** - Prepare AWS EC2 Instance, create SSH key credentials, extend CI pipeline with deploy step
- **cd-deploy-application-from-jenkins-pipeline-on-ec2-instance-automatically-with-docker-compose** - Install Docker Compose on EC2, create docker-compose.yml, configure Jenkins pipeline
- **complete-the-cicd-pipeline-docker-compose-dynamic-versioning** - Complete CI/CD project with version increment, build artifact, build and push Docker image, deploy with Docker Compose
- **interacting-with-aws-cli** - Install and configure AWS CLI, create EC2 Instance, create IAM resources, list and browse AWS resources

### Module 10: Container Orchestration with Kubernetes
- **deploy-mongodb-and-mongo-express-into-local-k8s-cluster** - Setup local K8s cluster with Minikube, deploy MongoDB and MongoExpress with ConfigMap and Secret
- **install-a-stateful-service-mongodb-on-kubernetes-using-helm** - Create managed K8s cluster with Linode Kubernetes Engine, deploy replicated MongoDB service using Helm chart
- **deploy-mosquitto-message-broker-with-configmap-and-secret-volume-types** - Define configuration and passwords for Mosquitto message broker with ConfigMap and Secret Volume types
- **deploy-our-web-application-in-k8s-cluster-from-private-docker-registry** - Create Secret for credentials, configure Docker registry secret, deploy web application from private registry
- **deploy-microservices-application-in-kubernetes-with-production-security-best-practices** - Create K8s manifests for Deployments and Services, deploy microservices to Linode's managed Kubernetes cluster
- **create-helm-chart-for-microservices** - Create shared Helm Chart for all microservices, reuse common Deployment and Service configurations
- **deploy-microservices-with-helmfile** - Deploy Microservices with Helm and Helmfile

### Module 11: Kubernetes on AWS - EKS
- **create-aws-eks-cluster-with-a-node-group** - Configure IAM Roles, create VPC with Cloudformation Template, create EKS cluster, create Node Group, configure Auto-Scaling
- **create-eks-cluster-with-fargate-profile** - Create Fargate IAM Role, create Fargate Profile, deploy example application using Fargate profile
- **create-eks-cluster-with-eksctl** - Create EKS cluster using eksctl tool to reduce manual effort
- **cd-deploy-to-eks-cluster-from-jenkins-pipeline** - Install kubectl and aws-iam-authenticator, create kubeconfig file, add AWS credentials, extend Jenkinsfile
- **cd-deploy-to-lke-cluster-from-jenkins-pipeline** - Create K8s cluster on LKE, install kubectl as Jenkins Plugin, adjust Jenkinsfile
- **complete-cicd-pipeline-with-eks-and-private-dockerhub-registry** - Write K8s manifest files, integrate deploy step in CI/CD pipeline to deploy from DockerHub private registry
- **complete-cicd-pipeline-with-eks-and-aws-ecr** - Create private AWS ECR Docker repository, adjust Jenkinsfile, integrate deploying to K8s cluster from AWS ECR

### Module 12: Infrastructure as Code with Terraform
- **automate-aws-infrastructure** - Create TF project to automate provisioning AWS Infrastructure and components (VPC, Subnet, Route Table, Internet Gateway, EC2, Security Group)
- **modularize-project** - Divide Terraform resources into reusable modules
- **terraform-aws-eks** - Automate provisioning EKS cluster with Terraform
- **complete-cicd-with-terraform** - Integrate provisioning stage into complete CI/CD Pipeline to automate provisioning server
- **configure-a-shared-remote-state** - Configure Amazon S3 as remote storage for Terraform state

### Module 13: Programming with Python
- **write-countdown-application** - Write application that accepts user input of goal and deadline, print remaining time
- **automation-with-python** - Write application that reads spreadsheet file and process/manipulate the spreadsheet
- **api-request-to-gitlab** - Write application that talks to GitLab API and lists all public GitLab repositories for specified user

### Module 14: Automation with Python
- **health-check-ec2-status-checks** - Create EC2 Instances with Terraform, write Python script to fetch EC2 statuses, extend to continuously check status
- **automate-configuring-ec2-server-instances** - Write Python script that automates adding environment tags to all EC2 Server instances
- **automate-displaying-eks-cluster-information** - Write Python script that fetches and displays EKS cluster status and information
- **data-backup-restore** - Write Python scripts to automate creating backups for EC2 Volumes, clean up old snapshots, restore EC2 Volumes
- **website-monitoring-and-recovery** - Create server on cloud platform, install Docker, write Python scripts for monitoring, email notifications, automatic restart

### Module 15: Configuration Management with Ansible
- **automate-nodejs-application-deployment** - Create Server on DigitalOcean, write Ansible Playbook to install technologies, create Linux user, deploy NodeJS application
- **automate-nexus-deployment** - Create Server on DigitalOcean, write Ansible Playbook to create Linux user for Nexus, configure server, install and deploy Nexus
- **ansible-docker** - Create AWS EC2 Instance with Terraform, write Ansible Playbook to install Docker and Docker Compose, copy docker-compose file, start containers
- **ansible-integration-in-terraform** - Create Ansible Playbook for Terraform integration, adjust Terraform configuration to execute Ansible Playbook automatically
- **configure-dynamic-inventory** - Create EC2 Instance with Terraform, write Ansible AWS EC2 Plugin to dynamically set inventory of EC2 servers
- **automate-kubernetes-deployment** - Create EKS cluster with Terraform, write Ansible Play to deploy application in new K8s namespace
- **ansible-integration-in-jenkins** - Create dedicated servers for Jenkins and Ansible Control Node, write Ansible Playbook, configure Jenkins to execute playbook
- **structure-playbooks-with-ansible-roles** - Break up large Ansible Playbooks into smaller manageable files using Ansible Roles

### Module 16: Monitoring with Prometheus
- **install-prometheus-stack-in-kubernetes** - Setup EKS cluster using eksctl, deploy Prometheus, Alert Manager and Grafana using Helm chart
- **configure-alerting-for-our-application** - Configure Monitoring Stack to notify when CPU usage > 50% or Pod cannot start, configure Alert Rules and Alertmanager
- **configure-monitoring-for-a-third-party-application** - Monitor Redis using Prometheus Exporter, deploy Redis service and exporter, configure Alert Rules, import Grafana Dashboard
- **configure-monitoring-for-own-application** - Configure NodeJS application to collect & expose Metrics with Prometheus Client Library, deploy to Kubernetes cluster, configure Prometheus to scrape metrics

## 🚀 Quick Start

Each repository in the `repos/` folder is a complete, standalone project. To get started:

1. **Navigate to any repository:**
   ```bash
   cd repos/[repository-name]
   ```

2. **Copy environment variables:**
   ```bash
   cp .env.example .env
   ```

3. **Edit the `.env` file with your actual values**

4. **Follow the README.md in each repository for specific instructions**

## 📁 Repository Structure

Each repository includes:
- **README.md** - Project description and quickstart instructions
- **.env.example** - Environment variables template
- **.gitignore** - Language-specific ignore patterns
- **config/** - Configuration files that read from environment variables
- **Technology-specific files** (Dockerfile, Jenkinsfile, Kubernetes manifests, etc.)

## 🛠️ Technologies Covered

- **Cloud Platforms**: AWS, DigitalOcean, Linode
- **Containers**: Docker, Docker Compose
- **Orchestration**: Kubernetes, Helm, EKS
- **CI/CD**: Jenkins, GitLab, Webhooks
- **Infrastructure as Code**: Terraform, Ansible
- **Programming**: Java (Gradle/Maven), Node.js, Python
- **Databases**: MongoDB, Redis
- **Monitoring**: Prometheus, Grafana
- **Artifact Management**: Nexus, Docker Registry

## 📋 Prerequisites

- Git
- Docker (for containerized projects)
- Python 3.x (for Python projects)
- Java 11+ (for Java projects)
- Node.js (for Node.js projects)
- kubectl (for Kubernetes projects)
- terraform (for Terraform projects)
- ansible (for Ansible projects)

## 🔐 Security Notes

- All repositories use environment variables for secrets
- No hardcoded credentials in any files
- `.env.example` files contain placeholder values only
- Always review and update environment variables before deployment

## 📖 Learning Path

The projects are organized by modules, progressing from basic cloud concepts to advanced DevOps practices:

1. **Modules 5-6**: Cloud basics and artifact management
2. **Module 7**: Container fundamentals with Docker
3. **Module 8**: CI/CD automation with Jenkins
4. **Module 9**: AWS services and deployment
5. **Module 10**: Kubernetes orchestration
6. **Module 11**: Advanced Kubernetes on AWS (EKS)
7. **Module 12**: Infrastructure as Code with Terraform
8. **Module 13**: Python programming fundamentals
9. **Module 14**: Python automation and AWS integration
10. **Module 15**: Configuration management with Ansible
11. **Module 16**: Monitoring and observability

## 🤝 Contributing

Each repository is designed to be self-contained and ready for immediate use. Feel free to:

- Customize the configurations for your specific needs
- Add additional features or integrations
- Share improvements and best practices
- Create additional modules or projects

## 📄 License

This project is licensed under the MIT License - see the individual repository README files for details.

---

**Happy DevOps Learning! 🚀** 
