# PetClinic on Kubernetes

This repository contains the deployment of the **PetClinic** application on a Kubernetes cluster. It demonstrates the use of Kubernetes for orchestrating containerized workloads, showcasing concepts such as scaling, service discovery, and deployment management.

---

## Repository Overview

- **Application**: PetClinic (a sample application demonstrating containerized microservices).
- **Environment**: Deployed on a Kubernetes cluster.
- **Tools Used**:
  - Kubernetes for orchestration.
  - Docker for containerization.
  - CI/CD pipelines for deployment automation.
  - Monitoring tools (optional integration).

---

## Repository Link

Access the repository here: [PetClinic-on-Kubernetes](https://github.com/iamtalhajalil/PetClinic-on-Kubernetes.git)

---

## How to Use

### Prerequisites
1. **Kubernetes Cluster**: Ensure you have a running Kubernetes cluster (e.g., Minikube, GKE, EKS, or AKS).
2. **kubectl**: Command-line tool for interacting with the cluster.
3. **Docker**: For building and managing container images.

### Steps to Deploy
1. Clone the repository:
   ```bash
   git clone https://github.com/iamtalhajalil/PetClinic-on-Kubernetes.git
   ```
2. Navigate to the repository directory:
   ```bash
   cd PetClinic-on-Kubernetes
   ```
3. Build the Docker images for the application (if not already built):
   ```bash
   docker build -t petclinic:latest .
   ```
4. Deploy the application to Kubernetes:
   ```bash
   kubectl apply -f k8s-manifests/
   ```
5. Check the status of the pods and services:
   ```bash
   kubectl get pods
   kubectl get services
   ```
6. Access the application using the external IP of the service or via port-forwarding:
   ```bash
   kubectl port-forward svc/petclinic 8080:8080
   ```

---

## What I Have Learned in DevOps Course

### Introduction to DevOps
- **DevOps Overview**: Principles of collaboration between development and operations teams for efficient software delivery.
- **Benefits of DevOps**: Faster deployments, improved collaboration, and higher software quality through automation.

### CI/CD Pipelines
- **Continuous Integration (CI)**: Automating code integration from multiple contributors.
- **Continuous Delivery (CD)**: Ensuring automatic testing and preparation for production deployment.
- **Tools Used**: Jenkins, GitLab CI/CD, CircleCI.

### Infrastructure as Code (IaC)
- **Concept**: Managing and provisioning infrastructure using machine-readable configuration files.
- **Tools**: Terraform, AWS CloudFormation, Ansible.

### Monitoring and Logging
- **Monitoring Tools**: Prometheus, Grafana, Nagios.
- **Logging Tools**: ELK Stack (Elasticsearch, Logstash, Kibana).

### Containerization and Orchestration
- **Docker**: For packaging applications into portable containers.
- **Kubernetes**: For managing and scaling containerized applications.

---

## Blogs Related to the Project

### Blog 1: Using Knative with Docker
- Explores the transition from containerized workloads to serverless architectures using **Knative** and **Docker**.
- Key highlights:
  - Knative provides serverless features such as auto-scaling and reduced operational overhead.
  - Demonstrates deploying a Flask application containerized with Docker on Knative.
- [Read More](#)

### Blog 2: Docker Networking
- Explains how Docker enables communication between containers using various networking drivers.
- Key highlights:
  - Overview of bridge, host, overlay, and none networks.
  - Best practices for designing scalable and secure container networks.
- [Read More](#)

---

## Features of the Deployment
- **Scalability**: Kubernetes enables horizontal scaling of the PetClinic application.
- **Service Discovery**: Uses Kubernetes Services for internal communication.
- **Rolling Updates**: Supports zero-downtime deployment of new application versions.

---

## Contributing
Contributions are welcome! Please create an issue or submit a pull request to contribute to this project.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact
For any queries or feedback, please contact the repository owner.
