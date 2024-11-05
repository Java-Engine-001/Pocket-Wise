## Project Overview

This project is a fintech microservices-based web application that enables users to perform essential financial transactions, such as user registration, logging in, topping up balances, and transferring funds securely through virtual wallets. Leveraging a modular microservices architecture, this application ensures scalability, security, and a smooth user experience, offering efficient user account and wallet management.

## Tech Stack

![Java](https://img.shields.io/badge/Java-17%2B-blue)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.2.0-green)
![Spring Cloud](https://img.shields.io/badge/Spring%20Cloud-2023.0.0-lightgrey)
![Wiremock](https://img.shields.io/badge/Testing-Wiremock-yellow)
![JUnit](https://img.shields.io/badge/Testing-JUnit-yellowgreen)
![Integration Tests](https://img.shields.io/badge/Testing-Integration%20Tests-important)
![OpenFeign](https://img.shields.io/badge/OpenFeign-Flexible%20Service%20Calls-ff69b4)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Minikube-blueviolet)
![Docker](https://img.shields.io/badge/Docker-Containerization-blue)
![Zipkin](https://img.shields.io/badge/Zipkin-Distributed%20Tracing-9cf)
![Logbook](https://img.shields.io/badge/Logbook-Centralized%20Logging-orange)
![Micrometer](https://img.shields.io/badge/Micrometer-Metrics%20Monitoring-ff66b2)
![Swagger](https://img.shields.io/badge/Swagger-API%20Docs-brightgreen)
![Microservice Architecture](https://img.shields.io/badge/Architecture-Microservices-red)
![DDD](https://img.shields.io/badge/Design%20Pattern-Domain%20Driven%20Design-ff69b4)
![DDT](https://img.shields.io/badge/Testing%20Pattern-Data%20Driven%20Testing-blue)
![Value Objects](https://img.shields.io/badge/Pattern-Value%20Objects-lightgrey)

## Architecture Patterns

- **Microservice Architecture** – Modular design with clearly defined service boundaries.
- **Domain-Driven Design (DDD)** – Emphasizes business domain logic separation.
- **Data-Driven Testing (DDT)** – Ensures comprehensive testing coverage.
- **Value Objects** – Maintains immutability and enhances code readability.

## Key Features

- User Registration and Authentication – Secure registration and login functionality.
- Balance Top-Up – Enables users to add funds to their virtual wallets.
- Fund Transfer – Allows secure and efficient transfer of funds between users.
- Detailed Transaction History – View complete transaction records for user reference.
- Comprehensive API Documentation – Enables seamless integration and service use.
  
![image](https://github.com/user-attachments/assets/ef4fc984-6d38-4ed6-a02d-bd360a94de39)

## Service Module Structure

Each module in the application adheres to microservices principles, with distinct responsibilities and clear separation:

### Auth Module
- `auth-sdk`: An SDK for integrating authentication features across modules.
- `auth-api`: Contains API interfaces and definitions for authentication processes.
- `auth-client`: Uses OpenFeign for remote authentication calls.
- `auth-service`: The core, runnable Spring application for user authentication and authorization.

### User Module
- `user-api`: Contains API definitions and interfaces for user operations.
- `user-client`: Facilitates remote calls for user-related actions.
- `user-service`: Manages core user operations, including registration and information retrieval.

### Wallet Module
- `wallet-api`: Defines API interfaces for wallet management and transactions.
- `wallet-client`: Feign client for seamless wallet-related interactions.
- `wallet-service`: Handles wallet functions such as creating wallets, topping up, and fund transfers.

Each module is version-controlled as a Maven variable, allowing consistent updates across the project and reducing manual maintenance efforts.

## My Contribution

In this project, I led the DevOps and Microservices aspects, building a robust deployment pipeline and containerizing the application with Docker. I deployed and managed the microservices in Kubernetes (with Minikube for local development), ensuring each service was scalable and secure. For observability, I implemented Zipkin for distributed tracing, Logbook for centralized logging, and Micrometer for metrics monitoring, providing a clear view of system health and performance. My contributions helped create a flexible, production-ready application, fully integrated with CI/CD workflows for efficient deployment and maintenance. 
