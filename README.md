# Shopping App (Flask + MySQL + HAPROXY) using Docker Compose

This project demonstrates a simple shopping web application using **Flask**, **MySQL**, and **NGINX**, all containerized using **Docker Compose**.

## 🧱 Components

- **Flask App**: The backend application
- **MySQL**: Relational database to store shopping data
- **HAProxy**: Acts as a reverse proxy and load balancer to route traffic across the Flask containers


## 🚀 Quick Start

### 1. Build Docker images


### Build the Flask application:

docker build -t arun1278/shopping-application:v1 .

### Build the HAPROXY proxy:


docker build -t arun1278/shopping-haproxy:v1 .

### 2. To check the full config being used:

docker compose config

### 3 Start the containers

docker compose up -d


🧹 Management Commands

Stop all services:

docker compose down

View logs:

docker compose logs -f

Rebuild containers:

docker compose up -d --build




