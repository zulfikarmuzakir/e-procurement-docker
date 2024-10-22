# E-Procurement Docker

This repository contains Docker configuration for the E-Procurement application, combining frontend and backend services.

## Prerequisites

- Docker
- Docker Compose
- Git

## Clone and Setup

### Method 1: Clone with submodules (Recommended)
```bash
git clone --recursive git@github.com:zulfikarmuzakir/e-procurement-docker.git
cd e-procurement-docker
```

### Method 2: Clone and initialize submodules manually
```bash
git clone git@github.com:zulfikarmuzakir/e-procurement-docker.git
cd e-procurement-docker
git submodule init
git submodule update
```

## Running the Application

1. Build and start the containers:
```bash
docker-compose up --build
```

2. Access the applications:
- Frontend: http://localhost:3000
- Backend API: http://localhost:8080
- Database: localhost:5433 (local) | postgres:5432 (docker)

## Services

- Frontend: React application
- Backend: Go API
- Database: PostgreSQL

## Development

To update submodules to their latest versions:
```bash
git submodule update --remote
```