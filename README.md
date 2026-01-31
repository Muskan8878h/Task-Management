# Task-Management (Microservices Architecture)

A **Spring Boot–based Task Management system** built using **Microservices Architecture**.  
This project demonstrates backend design using **API Gateway**, **Authentication**, and multiple independent services.

---

## 📌 Project Overview

This project is structured as a **multi-module microservices system**, where each service has a specific responsibility and can run independently.

**Best suited for:**
- Learning Spring Boot Microservices
- Understanding API Gateway concepts

---

## 🔹 Microservices Description

### 1️⃣ API Gateway
- Routes requests to backend services
- Runs on **port 8085**

### 2️⃣ Auth Service
- Handles authentication & authorization
- Manages user credentials
- Can be extended with JWT

### 3️⃣ Employee Service
- Manages employee-related data
- CRUD operations for employees

### 4️⃣ Task Service
- Manages task assignments
- Task creation, updates, and tracking

---

##  Tech Stack

- Java 17
- Spring Boot
- Spring Data JPA
- Hibernate
- MySQL
- Maven
- Embedded Tomcat

---

##  Prerequisites

Make sure the following are installed:
- Java 17+
- Maven
- MySQL (running on port 3306)
- IDE (IntelliJ / VS Code / Eclipse)

---

##  Database Setup

1. Start MySQL
2. Create databases:

# sql
`CREATE DATABASE ems_auth;
CREATE DATABASE ems_employee;
CREATE DATABASE ems_task;`

---

### ▶️ How to Run the Project

# 1. Run Auth Service
`cd auth-service
mvn spring-boot:run`

# 2. Run Employee Service
`cd employee-service
mvn spring-boot:run`

# 3. Run Task Service
`cd task-service
mvn spring-boot:run`

# 4. Run API Gateway
`cd api-gateway
mvn spring-boot:run`

###  Access URLs
`http://localhost:8085/signup.html`

---

### Future Enhancements

- JWT-based authentication
- Spring Cloud Gateway
- Docker 
- Centralized logging
- Frontend integration

---

### If you like this project

> Give it a ⭐ on GitHub and feel free to fork & improve it!
