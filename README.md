## Multi-Service Application with Docker Compose

This project demonstrates a clean Docker Compose setup with multiple services working together: an application, MySQL database, Redis cache, and an Nginx reverse proxy.
It is designed to showcase containerization, service orchestration, networking, and environment-based configuration.

## 🔧 Services
1. Application
Main backend service
Reads configuration from .env
Connects to MySQL and Redis

2. MySQL
Stores application data
Credentials defined in .env
Uses a persistent Docker volume

3. Redis
In-memory cache service
Internal-only (not exposed externally)

5. Nginx Reverse Proxy
Routes external traffic to the application
Acts as the public entry point

## 🚀 Running the Project

Start all services:
docker-compose up --build

Stop and remove resources:
docker-compose down -v

## 📁 Project Structure
app/                 
reverse-proxy/      
docker-compose.yml  
.env                


