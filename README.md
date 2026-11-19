
# Task Manager REST API

A RESTful Task Management API built with Java, Spring Boot, Spring Security, MySQL, and JWT Authentication.

## About the Project

This project is a backend REST API designed to manage users and their tasks. It follows a layered architecture to keep the application organized, maintainable, and easy to extend.

## Technologies Used

- Java 21
- Spring Boot
- Spring Security
- Spring Data JPA
- MySQL
- JWT Authentication
- Maven
- Lombok
- ModelMapper
- Postman

## Features

- User registration
- User login
- Password encryption using BCrypt
- JWT-based authentication
- User management
- RESTful API endpoints
- Input validation
- Global exception handling
- MySQL database integration

## Project Architecture

Controller → Service → Repository → Database

## Getting Started

### Prerequisites

- Java 21
- MySQL
- Maven
- IntelliJ IDEA (recommended)

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/MadushaThathsara/task-manager-rest-api.git
   ```

2. Open the project in IntelliJ IDEA.

3. Create a MySQL database named `task_manager`.

4. Configure environment variables in your IDE:

   - `DB_PASSWORD` – Your MySQL password
   - `JWT_SECRET` – A secure Base64-encoded secret key (at least 32 random bytes)

5. Run the Spring Boot application.

The application runs at:

`http://localhost:8080`

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/users/register` | Register a new user |
| POST | `/api/auth/login` | Login and receive JWT |
| GET | `/api/users` | Get all users |
| GET | `/api/users/{id}` | Get a user by ID |
| DELETE | `/api/users/{id}` | Delete a user |

**Note:** Protected endpoints require a valid JWT access token.

## Security

- Passwords are stored using BCrypt hashing.
- JWT secrets and database passwords are managed through environment variables.
- Sensitive configuration values are not committed to the repository.

## Testing

API endpoints can be tested using Postman.

## Author

**Madusha Thathsara Abeygunasekara**

GitHub: [MadushaThathsara](https://github.com/MadushaThathsara)
