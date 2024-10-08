# J-Run Project
* Technical Specifications Document: https://github.com/megahertz-uz/gat-deployment/blob/main/Technical%20Specification.pdf
* This repository contains only docker-compose files and GH Actions CI/CD files for deployment. Source codes of app in:
* https://github.com/megahertz-uz/gat-backend
* https://github.com/megahertz-uz/gat-frontend


# J-Run Deployment

This repository contains the infrastructure configuration and deployment scripts for the J-Run platform. The infrastructure is designed to be scalable, secure, and robust, utilizing modern cloud-native technologies.

## Infrastructure Overview

The J-Run platform infrastructure consists of the following components:

- **Redis**: Used for caching to improve response times and reduce database load.
- **MinIO**: Provides object storage for managing file uploads and large datasets.
- **PostgreSQL**: Serves as the primary relational database for managing structured data.
- **Traefik**: Acts as the load balancer, managing traffic routing for backend services.

## Infrastructure Diagram

Below is the infrastructure architecture for J-Run:

**Infrastructure Scheme:**
![Infrastructure Diagram](https://s01.pic4net.com/di-BUM3JI.png)

## Key Components

1. **Redis**: In-memory data store used for caching frequently accessed data to enhance performance.
2. **MinIO**: S3-compatible object storage for handling user uploads and binary data.
3. **PostgreSQL**: The relational database that stores user information, service data, and other relational entities.
4. **Traefik**: A reverse proxy and load balancer that routes incoming traffic to the appropriate backend services in a dynamic and efficient manner.

## Deployment Overview

We use Kubernetes and Docker Swarm to orchestrate the deployment of the infrastructure, ensuring high availability and scalability.

### Tools and Technologies

- **Docker**: For containerizing all services.
- **Traefik**: As the ingress controller and load balancer.

## Deployment Process
Fully automatized via CI/CD