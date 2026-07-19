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

---

# 🐳 Docker Architecture

Sociopedia is fully containerized using Docker following production-ready best practices. Each service runs in its own isolated container while communicating through a dedicated Docker network.

## 🚀 Docker Container Architecture

```mermaid
flowchart LR

Developer["👨‍💻 Developer"]

Dockerfile["📄 Dockerfile"]

Build["🔨 Docker Build"]

Frontend["⚛ React Image"]

Backend["🚀 Node Image"]

Compose["🐳 Docker Compose"]

Network["🌐 Docker Network"]

Containers["📦 Running Containers"]

Developer --> Dockerfile

Dockerfile --> Build

Build --> Frontend

Build --> Backend

Frontend --> Compose

Backend --> Compose

Compose --> Network

Network --> Containers

style Developer fill:#2563eb,color:#fff
style Dockerfile fill:#16a34a,color:#fff
style Build fill:#9333ea,color:#fff
style Frontend fill:#61DAFB,color:#000
style Backend fill:#339933,color:#fff
style Compose fill:#2496ED,color:#fff
style Network fill:#0891b2,color:#fff
style Containers fill:#f97316,color:#fff
```

---

# 🏗 Multi-Stage Docker Build

The frontend is built using a multi-stage Docker build to reduce image size and improve production performance.

```mermaid
flowchart LR

Source["📁 Source Code"]

Node["⚙ Node Builder"]

Install["📦 npm install"]

Build["🔨 npm run build"]

Nginx["🟢 Nginx Image"]

Production["🚀 Production Container"]

Source --> Node

Node --> Install

Install --> Build

Build --> Nginx

Nginx --> Production

style Source fill:#2563eb,color:#fff
style Node fill:#339933,color:#fff
style Install fill:#16a34a,color:#fff
style Build fill:#9333ea,color:#fff
style Nginx fill:#009639,color:#fff
style Production fill:#2496ED,color:#fff
```

---

# 🌍 Docker Compose Architecture

Docker Compose orchestrates all application services using a single configuration file.

```mermaid
flowchart TD

Compose["🐳 Docker Compose"]

Frontend["⚛ React"]

Backend["🚀 Express"]

Nginx["🟢 Nginx"]

Mongo["☁ MongoDB Atlas"]

Compose --> Frontend

Compose --> Backend

Compose --> Nginx

Backend --> Mongo

Nginx --> Frontend

Nginx --> Backend

style Compose fill:#2496ED,color:#fff
style Frontend fill:#61DAFB,color:#000
style Backend fill:#339933,color:#fff
style Nginx fill:#009639,color:#fff
style Mongo fill:#13AA52,color:#fff
```

---

# 🌐 Nginx Reverse Proxy

Nginx acts as the entry point for every incoming request and intelligently routes traffic to the appropriate service.

## Request Routing

```mermaid
flowchart LR

User["👨 User"]

Nginx["🟢 Nginx"]

React["⚛ React"]

API["🚀 Express API"]

Atlas["☁ MongoDB Atlas"]

User --> Nginx

Nginx -->|"/"| React

Nginx -->|"/api"| API

API --> Atlas

style User fill:#2563eb,color:#fff
style Nginx fill:#009639,color:#fff
style React fill:#61DAFB,color:#000
style API fill:#339933,color:#fff
style Atlas fill:#13AA52,color:#fff
```

---

# 🔒 Container Security

Production containers follow Docker security best practices.

```mermaid
flowchart TB

Docker["🐳 Docker"]

User["👤 Non-root User"]

Health["❤️ Health Check"]

Env["🔐 Environment Variables"]

Network["🌐 Private Network"]

Docker --> User

Docker --> Health

Docker --> Env

Docker --> Network

style Docker fill:#2496ED,color:#fff
style User fill:#16a34a,color:#fff
style Health fill:#dc2626,color:#fff
style Env fill:#9333ea,color:#fff
style Network fill:#0891b2,color:#fff
```

### Security Features

- ✅ Non-root containers
- ✅ Environment variables
- ✅ Health check endpoint
- ✅ Docker network isolation
- ✅ Production images
- ✅ Lightweight containers

---

# 🌐 Docker Networking

All services communicate through a dedicated isolated Docker bridge network.

```mermaid
flowchart LR

Client["👨 User"]

Bridge["🌐 Docker Bridge Network"]

Nginx["🟢 Nginx"]

Frontend["⚛ React"]

Backend["🚀 Express"]

Mongo["☁ MongoDB Atlas"]

Client --> Bridge

Bridge --> Nginx

Nginx --> Frontend

Nginx --> Backend

Backend --> Mongo

style Client fill:#2563eb,color:#fff
style Bridge fill:#0891b2,color:#fff
style Nginx fill:#009639,color:#fff
style Frontend fill:#61DAFB,color:#000
style Backend fill:#339933,color:#fff
style Mongo fill:#13AA52,color:#fff
```

---

# 💾 Persistent Storage

Application data remains safe using Docker volumes.

```mermaid
flowchart LR

Container["📦 Containers"]

Volume["💾 Docker Volume"]

Database["🗄 Local MongoDB"]

Container --> Volume

Volume --> Database

style Container fill:#2496ED,color:#fff
style Volume fill:#9333ea,color:#fff
style Database fill:#13AA52,color:#fff
```

---

# ☁ MongoDB Atlas Integration

The backend securely communicates with MongoDB Atlas using encrypted cloud connections.

```mermaid
flowchart LR

Express["🚀 Express API"]

TLS["🔒 Secure TLS"]

Atlas["☁ MongoDB Atlas"]

Collections["📂 Collections"]

Express --> TLS

TLS --> Atlas

Atlas --> Collections

style Express fill:#339933,color:#fff
style TLS fill:#dc2626,color:#fff
style Atlas fill:#13AA52,color:#fff
style Collections fill:#9333ea,color:#fff
```

---

# 📂 Project Structure

```text
docker-project/
│
├── client/
│   ├── src/
│   ├── public/
│   ├── Dockerfile
│   └── package.json
│
├── server/
│   ├── controllers/
│   ├── routes/
│   ├── middleware/
│   ├── models/
│   ├── Dockerfile
│   └── package.json
│
├── nginx/
│   ├── nginx.conf
│   └── Dockerfile
│
├── docker-compose.yml
├── .env
├── README.md
└── dark_theme_ss.png
```

---

# 🛠 Technology Stack

## Frontend

- React.js
- Redux Toolkit
- Material UI

---

## Backend

- Node.js
- Express.js
- MongoDB
- Mongoose

---

## DevOps

- Docker
- Docker Compose
- Nginx
- Multi-Stage Docker Build
- Docker Networks
- Docker Volumes

---

## Cloud

- MongoDB Atlas
- DigitalOcean
- Vercel

---

---

# 🚀 Future Enhancements

The following features can be added in future versions:

- 🔄 GitHub Actions for automated CI/CD
- ☸️ Kubernetes container orchestration
- 📊 Prometheus & Grafana monitoring
- 🔒 HTTPS with Let's Encrypt
- 🌍 Multi-container production deployment
- 📦 Image optimization and caching
- 📈 Application performance monitoring
- 🔐 OAuth Authentication (Google/GitHub)
- 📱 Progressive Web App (PWA) support

---

# 🎯 Key Learning Outcomes

Through this project, I gained practical experience in:

- 🐳 Building production-ready Docker images
- 📦 Multi-stage Docker builds
- 🌐 Configuring Nginx as a reverse proxy
- 🔐 Running containers as a non-root user
- ❤️ Implementing container health checks
- 🌍 Managing Docker networks
- 💾 Using Docker volumes for persistent storage
- ☁️ Connecting applications to MongoDB Atlas
- ⚙️ Managing multi-container applications with Docker Compose
- 📁 Organizing production-ready project structures

---

# 👨‍💻 Author

**Saurav Kumar**

**B.Tech Computer Science Engineering**

🚀 Full Stack Developer | DevOps Enthusiast

### Connect with Me

- 💼 LinkedIn: https://www.linkedin.com/in/your-linkedin
- 🐙 GitHub: https://github.com/Saurav6200907210

---

# 🤝 Contributing

Contributions, issues, and feature requests are welcome.

If you'd like to improve this project:

1. Fork the repository
2. Create a new feature branch
3. Commit your changes
4. Push your branch
5. Open a Pull Request

---

# ⭐ Support

If you found this project helpful, please consider giving it a **⭐ Star** on GitHub.

Your support motivates me to build more production-ready open-source projects.

---

# 📜 License

This project is licensed under the **MIT License**.

---

<div align="center">

## 🚀 Thanks for Visiting!

### Built with ❤️ using React, Node.js, Express, MongoDB, Docker & Nginx

⭐ **Don't forget to Star this repository if you found it useful!**

</div>
