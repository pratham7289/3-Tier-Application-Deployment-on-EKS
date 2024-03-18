# 3-Tier-Application-Deployment-on-EKS

# Project Overview
This project involves deploying a three-tier application using containerization and Kubernetes on AWS EKS. The application consists of front-end and back-end components, both containerized using Docker, and utilizes MongoDB as the database. The deployment process includes setting up an EC2 instance, creating Docker images, pushing them to Amazon ECR, provisioning an EKS cluster, and configuring routing and load balancing for external access.

## Tech Stack

- **Frontend:**
  - React.js

- **Backend:**
  - Node.js

- **Database:**
  - MongoDB

- **Containerization:**
  - Docker

- **Orchestration:**
  - Kubernetes

- **Cloud Provider:**
  - Amazon Web Services (AWS)

- **AWS Services:**
  - EC2 (Elastic Compute Cloud)
  - ECR (Elastic Container Registry)
  - EKS (Amazon Elastic Kubernetes Service)
  - ALB (Application Load Balancer)

## Instructions

To complete the project outlined in the provided overview, follow these steps:

1. **Set up an EC2 instance:**
   - Launch an EC2 instance on AWS with the necessary permissions to interact with AWS services.

2. **Clone the repository:**
   - SSH into the EC2 instance.
   - Clone the repository containing both the front end and back-end code.

3. **Create Dockerfiles:**
   - Create Dockerfiles for both the front end (React.js) and back end (Node.js) applications.

4. **Build and run Docker containers:**
   - Build Docker images from the Dockerfiles.
   - Run Docker containers based on the built images.

5. **Install AWS CLI:**
   - Install AWS CLI on the EC2 instance.

6. **Push Docker images to ECR:**
   - Create an Elastic Container Registry (ECR) repository on AWS.
   - Authenticate Docker to the ECR.
   - Tag Docker images with the ECR repository URI.
   - Push Docker images to the ECR repository.

7. **Install Kubernetes tools:**
   - Install kubectl and eksctl on the EC2 instance.

8. **Create an EKS cluster:**
   - Use eksctl to create an Amazon EKS cluster.
   - Specify details like cluster name, region, node type, and node capacity.

9. **Create deployment and service manifests:**
   - Create YAML manifests for deploying the front end, back end, and MongoDB.
   - Define Kubernetes deployment and service configurations for each component.

10. **Create a secret for MongoDB credentials:**
    - Generate a secret file containing MongoDB credentials.

11. **Apply manifests to the EKS cluster:**
    - Use kubectl to apply the Kubernetes manifests to the EKS cluster.

12. **Set up internal routing and load balancing:**
    - Use Kubernetes services for internal communication.
    - Deploy an Ingress Controller for external access.
    - Use Helm to simplify the deployment of the Ingress Controller and define routing paths.

13. **Create an Ingress resource:**
    - Define rules for routing external traffic to the appropriate services inside the EKS cluster.

14. **Install AWS Load Balancer (ALB):**
    - Set up an Application Load Balancer (ALB) to direct traffic into the EKS cluster.

15. **Verify deployment:**
    - Access the deployed application through the ALB's DNS or IP address.
    - Test functionality and ensure that the application is accessible and working as expected.

By following these steps, you should have successfully completed the project and deployed a three-tier application using containerization and Kubernetes on AWS EKS, with proper internal communication, load balancing, and external access set up.
