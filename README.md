# User-Management-Project

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

## Overview

The **User Management System** is a full-stack web application designed to manage user accounts, roles, and permissions in an organized and secure manner. This system provides an intuitive interface for administrators to create, update, and manage user profiles while ensuring data integrity and security.

## Table of Contents

- [Features](#features)
- [Technologies](#technologies)
- [Architecture](#architecture)
- [Acknowledgements](#acknowledgements)

## Features

- **Role-Based Access Control**: Assign roles and permissions to users for granular access management.
- **User Registration and Management**: Create, update, and delete user profiles.
- **Secure Authentication**: Implemented using Spring Security with support for encrypted passwords.
- **Responsive UI**: Built with Angular and Bootstrap, ensuring compatibility across devices.
- **RESTful APIs**: Comprehensive API endpoints for managing users and roles.
- **Search and Filter**: Advanced search functionality to easily find users based on various criteria.
- **Audit Logging**: Track user activities for security and accountability.

## Technologies

### Backend
- **Java**: Core language for server-side development.
- **Spring Boot**: Framework for building the backend services.
- **Spring Security**: Provides authentication and authorization.
- **JPA/Hibernate**: For ORM and database interactions.
- **MySQL**: Relational database for storing user data.

### Frontend
- **Angular**: Frontend framework for building dynamic web applications.
- **TypeScript**: Strongly-typed superset of JavaScript used in Angular.
- **Bootstrap**: Ensures a responsive and mobile-friendly user interface.

## Architecture

The application follows a **multi-tier architecture** with a clear separation between the frontend, backend, and database layers.

### Backend
- **REST API**: Spring Boot serves as the backend, exposing RESTful endpoints for CRUD operations on users and roles.
- **Service Layer**: Business logic is encapsulated in the service layer, ensuring clean and maintainable code.
- **Repository Layer**: Interfaces with the database using JPA repositories.

### Frontend
- **Angular Components**: Modular components manage the user interface and handle user interactions.
- **Services**: Angular services communicate with the backend via HTTP.

### Database
- **MySQL Schema**: Contains tables for `users`, `roles`, and `permissions`.
- **Entity Relationships**: Utilizes JPA annotations to define relationships like `@OneToMany` and `@ManyToOne`.

 ## Acknowledgements
- **Spring Boot**: For simplifying backend development.
- **Angular**: For a powerful frontend framework.
- **MySQL**: For reliable and efficient database management.
- **Open Source Community**: For ongoing support and resources.

### Data Flow Diagram

```plaintext
+-----------+      +-----------+      +----------+      +-------+
| Frontend  | ---> |   REST    | ---> | Service  | ---> | MySQL |
|  Angular  |      |   API     |      |  Layer   |      |       |
+-----------+      +-----------+      +----------+      +-------+
