# Microservices-Based Student & School Management System

## Overview

This repository contains the source code for a Microservices-Based Student & School Management System. The system is designed to efficiently manage student and school information through a microservices architecture.

## Features

- **Microservices Architecture:** Utilized microservices for scalability and maintainability.
- **Service Discovery (Eureka):** Implemented Eureka for seamless service registration and discovery.
- **API Gateway (Spring Cloud Gateway):** Managed and routed requests efficiently between microservices.
- **Configuration Management (Config Server):** Centralized configuration management for enhanced flexibility.
- **Communication between Microservices (OpenFeign):** Enabled smooth communication between microservices.
- **Distributed Tracing (Zipkin):** Integrated Zipkin for enhanced visibility and debugging capabilities.

## Getting Started

### Prerequisites

- [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/javase-downloads.html)
- [Git](https://git-scm.com/)
- [Docker](https://www.docker.com/) (Optional: Required if using Docker for microservices)


### Installation Steps

1. **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/microservices-student-school.git
    ```

2. **Navigate to the project directory:**

    ```bash
    cd microservices-student-school
    ```

3. **Run the microservices:**

    - If using Docker:

        ```bash
        docker-compose up
        ```

    - If running each microservice individually, follow the instructions in their respective directories.

4. **Access the APIs:**

    - Open your preferred API client (e.g., [Postman](https://www.postman.com/)).

    - Example API endpoints and usage:

        - Retrieve all schools:
          ```
          GET http://localhost:8080/api/schools
          ```

        - Add a new student to a school:
          ```
          POST http://localhost:8080/api/schools/{schoolId}/students
          ```

        - Retrieve a school with all students:
          ```
          GET http://localhost:8080/api/schools/{schoolId}/students
          ```
