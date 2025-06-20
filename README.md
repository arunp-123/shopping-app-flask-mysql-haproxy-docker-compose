🛍️ Shopping App (Flask + MySQL + HAProxy) using Docker Compose
This project demonstrates a simple shopping web application using Flask, MySQL, and HAProxy, all containerized using Docker Compose.
🧱 Components
Flask App: The backend web application served via three replicas
MySQL: Relational database to store shopping product data
HAProxy: Acts as a reverse proxy and load balancer to route traffic across the Flask containers
🚀 Quick Start
1️⃣ Build Docker Images
✅ Build the Flask application image:
docker build -t arun1278/shopping-application:v1 .
✅ Build the HAProxy reverse proxy image:
docker build -t arun1278/shopping-haproxy:v1 .
2️⃣ View the full effective Docker Compose config:
docker compose config
3️⃣ Start All Containers
docker compose up -d
🔄 Useful Docker Management Commands
✅ Rebuild and restart all containers:
docker compose up -d --build
✅ Stop and remove all services:
docker compose down
✅ View real-time logs:
docker compose logs -f
