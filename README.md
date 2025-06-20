# 🛍️ Shopping App (Flask + MySQL + HAProxy) using Docker Compose

This project demonstrates a simple shopping web application using **Flask**, **MySQL**, and **HAProxy**, all containerized using **Docker Compose**.

---

## 🧱 Components

- **Flask App**: The backend web application served via three replicas
- **MySQL**: Relational database to store shopping product data
- **HAProxy**: Acts as a reverse proxy and load balancer to route traffic across the Flask containers

---

## 🚀 Quick Start

### 1️⃣ Build Docker Images

✅ Build the Flask application image:
```bash
docker build -t arun1278/shopping-application:v1 .
