# English Mock Test – Backend Service (Go)

A production-oriented RESTful backend service built with Go, designed to power a full English mock testing platform.

This project focuses on clean architecture, scalability, and maintainability — following backend engineering best practices.

---

## Project Goal

To design and implement a scalable backend system that:

* Handles mock test execution
* Calculates scores automatically
* Manages question banks
* Supports role-based authentication
* Serves both client and admin applications

---

## Architecture Overview

The backend follows a layered architecture:

```
HTTP Layer (Handler)
        ↓
Service Layer (Business Logic)
        ↓
Repository Layer (Data Access)
        ↓
MySQL
```

### Architectural Principles

* Clear separation of concerns
* Dependency injection
* Interface-driven design
* Stateless authentication (JWT)
* Middleware-based request pipeline
* Environment-based configuration

---

## Tech Stack

* **Go**
* **Gin** (HTTP framework)
* MySQL
* JWT Authentication
* RESTful API design
* Structured logging
* Environment configuration (.env)

---

## Core Backend Features

### Authentication & Authorization

* JWT-based authentication
* Access token validation middleware
* Role-based access control (User / Admin)
* Secure route grouping

### Exam Engine

* Timed mock test session handling
* Auto score calculation logic
* Persistent result storage
* Efficient question retrieval

### Admin System

* CRUD operations for question bank
* Test set creation and management
* User management
* Protected admin endpoints

---

## API Design

* RESTful route structure
* Versioned API (if applicable)
* Standardized JSON response format
* Centralized error handling
* Input validation & binding

Example:

```
POST   /api/v1/auth/login
GET    /api/v1/tests
POST   /api/v1/tests/submit
GET    /api/v1/admin/questions
```

---

## Backend Engineering Highlights

* Clean layered structure (handler → service → repository)
* Reusable middleware
* Centralized error handler
* Production mode configuration
* Proper HTTP status code usage
* Context-based request handling
* Transaction handling for critical operations

---

## Database Design

* Relational schema design
* Normalized tables
* Foreign key constraints
* Indexed columns for optimized queries
* Separation between test sessions and question bank

---

## Scalability Considerations

* Stateless API (horizontal scaling ready)
* JWT-based authentication (no server session storage)
* Modular service structure
* Easily extendable to microservices
* Ready for containerization (Docker-ready structure)

---

## Potential Improvements

* Redis caching layer
* Background job processing (e.g., result analytics)
* Rate limiting middleware
* CI/CD integration
* Load testing & performance benchmarking
* OpenAPI documentation

---

## What This Project Demonstrates

* Ability to design REST APIs in Go
* Clean architecture understanding
* Production mindset in backend development
* Authentication & authorization implementation
* Scalable system thinking

---

## Author

Luan
Backend-focused Go Developer

Interested in Backend / Platform Engineering roles.
