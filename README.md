# E-Procurement System

This project is an E-Procurement System built using a modern tech stack with Docker containerization.

## Project Structure

The project consists of three main components:

1. Backend API (Golang)
2. Frontend Application (React)
3. PostgreSQL Database

## Prerequisites

- Docker
- Docker Compose

## Getting Started

1. Clone the repository:

   ```
   git clone git@github.com:zulfikarmuzakir/e-procurement-docker.git
   cd e-procurement
   ```

2. Start the application:

   ```
   docker-compose up -d
   ```

3. Access the application:
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:8080

## Services

### PostgreSQL Database

- Port: 5433 (host) -> 5432 (container)
- User: root
- Password: password
- Database: e_procurement

### Backend API

- Port: 8080
- Depends on: PostgreSQL Database

### Frontend

- Port: 3000
- Depends on: Backend API


## Stopping the Application

To stop the application and remove the containers:

```
docker-compose down
```
