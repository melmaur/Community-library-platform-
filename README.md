# 🏛️ Community Library Platform

A full-stack library management system built in Java,
consisting of three independent but interconnected services
developed following the Scrum framework.

## 🗺️ Platform Overview

```
┌─────────────────────┐
│  Library Management  │  Java console app — book catalog management
│     (Project 1)      │  CSV persistent storage
└─────────┬───────────┘
          │
          ▼
┌─────────────────────┐
│   Library REST API   │  Spring Boot — exposes catalog via HTTP
│     (Project 2)      │  H2 database, full CRUD endpoints
└─────────┬───────────┘
          │
          ▼
┌─────────────────────┐
│   Booking System     │  Spring Boot — reservations management
│     (Project 3)      │  REST API + web frontend
└─────────────────────┘
```

## 🔗 Services

| Project | Description | Technologies | Repository |
|---|---|---|---|
| Library Management | Java console app for book catalog | Java, OOP, CSV, Git | [library-java](https://github.com/melmaur/library-java.git) |
| Library REST API | Spring Boot REST API for book catalog | Spring Boot, JPA, H2 | [todo-api](https://github.com/melmaur/todo-api.git) |
| Booking System | Full stack booking system with web UI | Spring Boot, JPA, H2, HTML/CSS/JS | [library-booking](https://github.com/melmaur/library-booking.git) |

## 🏗️ Architecture

Each service is independent but designed to work together as a microservices-inspired architecture:

- **Project 1** manages the book catalog locally via console
- **Project 2** exposes the catalog via REST API
- **Project 3** consumes the catalog and manages reservations via REST API and web frontend

## 🛠️ Technologies

- Java 21
- Spring Boot 3.5.13
- Spring Data JPA
- H2 In-memory Database
- Maven
- HTML / CSS / JavaScript
- Git & GitHub

## ⚙️ Agile Process

All three projects were developed following the **Scrum framework**:

- Work organized in Sprints with defined Sprint Goals
- User stories tracked in Product Backlogs
- Daily standup logs maintained throughout development
- Each Sprint concluded with a Review and Retrospective
- Full Scrum artifacts visible in each repository

> Developer holds a **Professional Scrum Master I (PSM I) certification issued by Scrum.org

## 🔮 Future Development

- **Spring Security** — user authentication and login
- **Role-based access control** — Admin vs User permissions
- **JUnit tests** — unit and integration testing
- **Docker** — containerization of all three services
- **React frontend** — upgrade web UI to a modern framework

## 🚀 How to Run

### Project 1 — Library Management
```
1. Open library-java in IntelliJ
2. Run Main.java
3. Use the console menu
```

### Project 2 — Library REST API
```
1. Open todo-api in IntelliJ
2. Run TodoApiApplication.java
3. API available at http://localhost:8080/api/todos
4. H2 console at http://localhost:8080/h2-console
```

### Project 3 — Booking System
```
1. Open library-booking in IntelliJ
2. Run LibraryBookingApplication.java
3. Web UI at http://localhost:8080
4. API at http://localhost:8080/api/bookings
5. H2 console at http://localhost:8080/h2-console
```

## 📁 Repository Structure

Each repository contains:
```
📄 README.md          → project documentation
📄 BACKLOG.md         → product backlog with user stories
📄 DAILY.md           → sprint daily standup log
📄 SPRINT_REVIEW.md   → sprint review
📄 RETROSPECTIVE.md   → sprint retrospective
📁 docs/screenshots   → Postman and frontend screenshots
📁 src/               → source code
```
