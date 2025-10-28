# Comment-Service-API

**Comment Management Microservice – Spring Boot 3.x, PostgreSQL & Redis Caching**

---

## 📌 Overview
Comment-Service-API is a standalone microservice designed to handle user comments for blogs, social apps, and product review platforms. It is built to be scalable, secure, and highly performant with Redis caching for frequently accessed comment data.

---

## 🚀 Features
- CRUD operations for comments
- PostgreSQL database with indexes for optimized filtering
- Redis caching for faster repeated content access
- Token-based authentication and anti-spam measures
- Modular, clean Spring Boot layered architecture
- Swagger/OpenAPI documentation for frontend integration
- Docker container deployment ready

---

## 🛠️ Tech Stack
| Component | Technology |
|----------|------------|
| Language | Java 17 |
| Framework | Spring Boot 3.x |
| Database | PostgreSQL |
| Cache | Redis |
| API Docs | Swagger / OpenAPI 3 |
| Security | Spring Security with Token Auth |
| Build | Maven |
| Deployment | Docker |

---

## 🧱 Architecture Diagram
![Architecture Diagram](architecture-diagram.png)

---

## ▶️ Setup & Run

### 1️⃣ Clone the repository
```bash
git clone https://github.com/sritam94/comment-service-api.git
cd comment-service-api
