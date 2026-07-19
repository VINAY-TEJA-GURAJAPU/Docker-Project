# 🚀 Sociopedia

<div align="center">

# 🌐 Production-Ready Dockerized MERN Application

### 🐳 Docker • 🌍 Nginx Reverse Proxy • ☁️ MongoDB Atlas • ⚡ Production Architecture

<p align="center">

![React](https://img.shields.io/badge/Frontend-React-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![Redux](https://img.shields.io/badge/State-Redux-764ABC?style=for-the-badge&logo=redux&logoColor=white)
![Material UI](https://img.shields.io/badge/UI-Material_UI-007FFF?style=for-the-badge&logo=mui&logoColor=white)
![NodeJS](https://img.shields.io/badge/Backend-Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Framework-Express-000000?style=for-the-badge&logo=express)
![MongoDB](https://img.shields.io/badge/Database-MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Docker](https://img.shields.io/badge/Container-Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Reverse_Proxy-Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![MongoDB Atlas](https://img.shields.io/badge/Cloud-MongoDB_Atlas-13AA52?style=for-the-badge&logo=mongodb)

</p>

</div>

---

# 📖 About Sociopedia

**Sociopedia** is a **production-ready full-stack social media platform** built using the MERN stack and containerized with Docker using enterprise deployment practices.

The project demonstrates how modern applications are packaged, secured, networked, and deployed using production-grade Docker techniques.

Instead of running services individually, the complete application is deployed using **Docker Compose**, **Nginx Reverse Proxy**, isolated Docker networks, persistent volumes, and MongoDB Atlas integration.

---

# ✨ Key Features

## 👥 Social Media Platform

- User Authentication
- JWT Authorization
- Create Posts
- Like & Comment
- Friend System
- Responsive UI

---

## ⚛ Frontend

- React.js
- Redux Toolkit
- Material UI
- Responsive Design
- Protected Routes
- API Integration

---

## 🚀 Backend

- Node.js
- Express.js
- JWT Authentication
- REST APIs
- Secure Middleware
- MongoDB Integration

---

## 🐳 Production Docker Features

- Multi-stage Docker Build
- Docker Compose
- Non-root Containers
- Health Checks
- Docker Networks
- Persistent Volumes
- Environment Variables
- Reverse Proxy
- Production Ready Images

---

# 🌐 Live Deployment

## Frontend

https://sociopedia-app.vercel.app

---

## Backend API

https://urchin-app-v2nci.ondigitalocean.app

---

# 🏗 High Level Architecture

```mermaid
flowchart LR

User["👨‍💻 User"]

Browser["🌐 Browser"]

Nginx["🟢 Nginx Reverse Proxy"]

Frontend["⚛ React Frontend"]

Backend["🚀 Express API"]

Atlas["☁ MongoDB Atlas"]

Browser --> Nginx

Nginx --> Frontend

Nginx --> Backend

Backend --> Atlas

style User fill:#2563eb,color:#fff
style Browser fill:#0ea5e9,color:#fff
style Nginx fill:#009639,color:#fff
style Frontend fill:#61DAFB,color:#000
style Backend fill:#339933,color:#fff
style Atlas fill:#13AA52,color:#fff
```

---

# 🏢 Enterprise System Architecture

```mermaid
flowchart TD

Client["👨 User"]

Internet["🌍 Internet"]

Nginx["🟢 Nginx Reverse Proxy"]

React["⚛ React Container"]

Express["🚀 Node API Container"]

Docker["🐳 Docker Network"]

Mongo["☁ MongoDB Atlas"]

Client --> Internet

Internet --> Nginx

Nginx --> React

Nginx --> Express

React --> Express

Express --> Docker

Docker --> Mongo

style Client fill:#2563eb,color:#fff
style Internet fill:#0891b2,color:#fff
style Nginx fill:#009639,color:#fff
style React fill:#61DAFB,color:#000
style Express fill:#339933,color:#fff
style Docker fill:#2496ED,color:#fff
style Mongo fill:#13AA52,color:#fff
```

---

# 🔄 Request Flow

```mermaid
flowchart LR

User["👨 User"]

Browser["🌐 Browser"]

Nginx["🟢 Nginx"]

Frontend["⚛ React"]

API["🚀 Express"]

Database["☁ MongoDB Atlas"]

Response["📄 JSON Response"]

User --> Browser

Browser --> Nginx

Nginx --> Frontend

Frontend --> API

API --> Database

Database --> Response

Response --> Frontend

Frontend --> User

style User fill:#2563eb,color:#fff
style Browser fill:#0891b2,color:#fff
style Nginx fill:#009639,color:#fff
style Frontend fill:#61DAFB,color:#000
style API fill:#339933,color:#fff
style Database fill:#13AA52,color:#fff
style Response fill:#9333ea,color:#fff
```

---

# 📸 Application Preview

## 🌙 Dark Theme UI

<img src="dark_theme_ss.png" width="1200">

---

## 🗄 Database Schema

<img src="server/sociopedia-schema.png" width="650">

---
