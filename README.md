# 🚀 Sociopedia – Production Ready Dockerized MERN App

A full-stack social media web application built using the MERN stack and containerized using Docker with production-level DevOps practices.

---

## 🌐 Live Deployment

- 🔗 Frontend (Vercel): https://sociopedia-app.vercel.app  
- 🔗 Backend API (DigitalOcean): https://urchin-app-v2nci.ondigitalocean.app  

---

## 🛠 Tech Stack

### 💻 Frontend
- React
- Redux Toolkit
- Material UI

### 🖥 Backend
- Node.js
- Express.js
- MongoDB (Mongoose)

### ⚙ DevOps & Infrastructure
- Docker
- Docker Compose
- Nginx (Reverse Proxy)
- MongoDB Atlas
- Multi-stage Docker builds
- Non-root container security
- Health checks
- Custom Docker network
- Volume persistence

---

## 🏗 Architecture Overview

User  
→ Nginx Reverse Proxy  
→ React Frontend  
→ Express Backend API  
→ MongoDB Atlas  

---

## 📂 Project Structure

project/
│
├── server/ # Backend (Node + Express)
├── client/ # Frontend (React)
├── nginx/ # Nginx configuration
├── docker-compose.yml
├── .env
└── README.md

---

## 🔐 Environment Variables

Create a `.env` file in the root directory:

PORT=5000
MONGO_URL=mongodb+srv://<username>:<password>@cluster.mongodb.net/sociopedia
JWT_SECRET=your_secret_key


⚠ Never commit `.env` to GitHub.

---

## 🐳 Running with Docker

### Build and Start Containers

docker-compose down -v
docker-compose up -d --build


### Access Application

http://localhost:5001

---

## 🛡 Production Features Implemented

- ✅ Dockerized frontend & backend
- ✅ Multi-stage React production build
- ✅ Secure backend container (non-root user)
- ✅ Reverse proxy using Nginx
- ✅ MongoDB Atlas cloud database integration
- ✅ Healthcheck endpoint monitoring
- ✅ Log rotation configuration
- ✅ Persistent Mongo volume
- ✅ Custom isolated Docker network
- ✅ Ready for zero-downtime scaling

---

## 🔄 Backend Health Endpoint

GET /health


Returns:

200 OK


---

## 📸 Snapshot

<img src="dark_theme_ss.png" width="1200">

---

## 🗄 MongoDB Schema

<img src="server/sociopedia-schema.png" width="600">

---

## 📈 Key Learning Outcomes

- Containerization best practices
- Handling native dependencies inside Docker
- Managing environment variables securely
- Solving networking & port conflicts
- Integrating cloud database (MongoDB Atlas)
- Production-ready backend configuration

---

## 🔮 Future Improvements

- CI/CD with GitHub Actions
- AWS EC2 Deployment
- HTTPS with Let's Encrypt
- Monitoring with Prometheus & Grafana
- Kubernetes Migration

---

## 🙏 Acknowledgments

This project was inspired by the fantastic tutorial by EdRoh:  
https://youtu.be/K8YELRmUb5o

---

## 👨‍💻 Author

Saurav Singh  
B.Tech CSE | Full Stack & DevOps Enthusiast
