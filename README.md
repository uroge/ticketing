# Ticketing Microservices Practice

This repository is a practice project for building a microservices-based application using Docker and Kubernetes. The goal is to gain hands-on experience with modern cloud-native development, including:

- **Microservices Architecture:** Each service is developed and deployed independently for scalability and maintainability.
- **Docker:** Containerization of services for consistent deployment across environments.
- **Kubernetes:** Orchestration and management of containers, including load balancing and service discovery.
- **AWS Integration:** Deployment of databases and container images on AWS infrastructure (ECR, RDS, etc.).
- **Load Balancing:** Using Kubernetes Ingress and NGINX for routing and balancing traffic between services.

## Current Services

- **Auth Service:** Handles user authentication and exposes user-related endpoints.

## Development Workflow

- Services are developed in TypeScript using Express.js.
- Dockerfiles are provided for containerization.
- Kubernetes manifests are used for deployment and service configuration.
- Skaffold is used for local development and deployment automation.

## Getting Started

1. Clone the repository.
2. Install dependencies for each service.
3. Use Docker and Skaffold to build and deploy locally.
4. Configure AWS credentials for pushing images and connecting to cloud databases.

## Future Plans

- Add more services (e.g., ticketing, payments).
- Integrate a cloud database (AWS RDS).
- Implement authentication and authorization.
- Set up CI/CD pipelines.

---

This project is for educational purposes and experimentation with cloud-native technologies.
