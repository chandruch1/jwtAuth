# JWT Authentication Backend

A secure Spring Boot REST API that implements JWT (JSON Web Token) based authentication and authorization. This project provides user registration, login, and protected endpoints using Spring Security and JWT.

## Features

- User Registration
- User Login
- JWT Authentication
- Protected APIs
- Spring Security Integration
- MySQL Database Support
- RESTful API Architecture

## Tech Stack

- Java 17
- Spring Boot
- Spring Security
- JWT
- MySQL
- Maven

## Getting Started

### Clone the Repository

Download the project source code from GitHub.

```bash
git clone https://github.com/your-username/jwt-auth-backend.git
```

### Navigate to the Project Directory

Move into the project folder.

```bash
cd jwt-auth-backend
```

### Build the Project

Download required dependencies and build the application.

```bash
mvn clean install
```

### Run the Application

Start the Spring Boot application.

```bash
mvn spring-boot:run
```

The application will be available at:

```text
http://localhost:8080
```

### Alternative: Run Using JAR File

Package the application:

```bash
mvn clean package
```

Run the generated JAR file:

```bash
java -jar target/*.jar
```

## API Endpoints

### Register User

```http
POST /api/auth/register
```

### Login User

```http
POST /api/auth/login
```

### Access Protected Endpoint

```http
GET /api/user/profile
Authorization: Bearer <JWT_TOKEN>
```

## Prerequisites

- Java 17+
- Maven
- MySQL
- Git

## Database Configuration

Update `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/your_database
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
```
