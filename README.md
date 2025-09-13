# Patient Management System with Microservices

**Presentation** : https://docs.google.com/presentation/d/1hJnGUnJCl5XHOlE1zWKqN73RZLYFykjIk3cXywc13g4/edit?usp=drive_link

**Demo Video** : https://drive.google.com/file/d/1nZukgCNBzn-q8UY_qNyJYiKDMAVxPceV/view?usp=sharing


This project features a **real-world, enterprise-level patient management system** built with production-ready **microservices**. It provides hands-on experience in **Java Spring Boot, Docker, and AWS cloud deployment**, including Infrastructure as Code.

## Project Description

The system offers a complete, **end-to-end understanding** of modern enterprise technologies, building features module by module. It simulates **full cloud deployment** on AWS, locally using localstack.

## Features

*   **Microservices Architecture:** Production-ready microservices using Java Spring Boot and Docker.
*   **Data Storage:** Uses **PostgreSQL** for data persistence and **H2 in-memory database** for local development.
*   **Inter-service Communication:** Implements **REST** and **gRPC** for efficient microservice interaction, and **Apache Kafka** for event-driven communication.
*   **API Gateway:** Built with **Spring Cloud Gateway** for request routing, load balancing, and handling cross-cutting concerns like security.
*   **Security:** Features **user authentication** and **API security** using a dedicated Auth Service with **JWT Bearer tokens**.
*   **Deployment Simulation:** Leverages **LocalStack** to simulate AWS infrastructure locally, using **Infrastructure as Code (IaC)** with AWS Cloud Development Kit (CDK) in Java.
*   **Automated Testing:** Includes **automated integration tests** to ensure reliability.
*   **API Documentation:** Generates **OpenAPI/Swagger UI** documentation for APIs.

## Technologies Used

*   **Backend:** Java, Spring Boot
*   **Containerization:** Docker
*   **Data Stores:** PostgreSQL, H2 Database
*   **Messaging:** Apache Kafka
*   **API Gateway:** Spring Cloud Gateway
*   **Communication:** REST, gRPC (with Protocol Buffers)
*   **Security:** Spring Security, JSON Web Tokens (JWT)
*   **Cloud Simulation:** LocalStack
*   **Infrastructure as Code:** AWS Cloud Development Kit (CDK) in Java, AWS CloudFormation
*   **Simulated AWS Services:** VPC, ECS (Fargate), RDS, MSK, ALB
*   **Development Tools:** IntelliJ IDEA Ultimate, Maven, Git
*   **Testing:** Rest Assured, JUnit Jupiter

## Prerequisites

*   **Basic Knowledge:** Java (variables, loops, classes, methods, OOP), Spring Boot, REST APIs, database concepts. Knowledge of microservices and Docker is helpful.
*   **Software:**
    *   **Java Development Kit (JDK) 21**
    *   **Docker Desktop**
    *   **IntelliJ IDEA Ultimate** (extended free trial available)
    *   **AWS Command Line Interface (CLI) v2**
    *   **LocalStack Desktop Application** (requires API key)

## Setup Instructions (Short Descriptions)

1.  **Install Prerequisites:** Ensure JDK 21, Docker Desktop, IntelliJ IDEA Ultimate, AWS CLI, and LocalStack Desktop are installed and configured.
2.  **Clone Project:** Obtain the project code from GitHub.
3.  **Local Development (Docker & PostgreSQL):** Run microservices in Docker containers, utilising PostgreSQL databases for persistence. Configure inter-service communication via REST, gRPC, and Kafka.
4.  **Kafka Topic Creation:** Use IntelliJ Kafka tools to create the `patient` topic for event streaming .
5.  **Deployment (LocalStack IaC):** Define AWS infrastructure using AWS CDK in Java within the `infrastructure` module. Build Docker images for microservices. Deploy the CloudFormation stack to LocalStack using the provided `localstack-deploy.sh` script.
6.  **Testing:** Use IntelliJ's built-in HTTP client for manual API testing. Run automated integration tests via the `integration-tests` module.
