# Dockerized Full-Stack Application

This repository contains the `docker-compose.yml` file for running a full-stack application with a PostgreSQL database, a backend, and a frontend using Docker Compose. Will 

## Services

The `docker-compose.yml` sets up the following services:

1. **PostgreSQL Database (`database`)**
   - Port: `5435` (mapped to container's `5432`)
   - Stores application data

2. **Backend (`backend`)**
   - Port: `8080`
   - Built from the `./Backend` directory
   - Handles business logic and API requests
   - Uses `Spring Boot` and connects to the PostgreSQL database

3. **Frontend (`frontend`)**
   - Port: `3000`
   - Built from the `./Frontend` directory
   - React-based user interface for interacting with the application

---

## Requirements

- Docker installed on your machine
- Docker Compose installed (included with Docker Desktop)
- Git (for cloning the repository)

---

## Setup Instructions

Assuming this is set up on an ubuntu virtual machine

1. Clone the repository:
2. Start the application:
   ```docker-compose up```
4. Connect to the VMs public ip address with port 3000
