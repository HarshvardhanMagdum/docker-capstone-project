Docker Capstone Project

Name: Harshvardhan Magdum

Trainer: Dr. Ankur Shrama

Course: Java Full Stack Development

Project Title: Multi-container Web Application using Docker


Description:
This project demonstrates a containerized 3-tier web application using Docker.
It includes:
1. Frontend - Nginx web server serving static HTML.
2. Backend - Python Flask application 
3. Database - MySQL database for persistent data storage.

Each service runs in its own container and communicates through a Docker network.
The application is orchestrated using Docker Compose and deployed with Docker Swarm.

Project Setup Instructions

1. Build Docker Images:
   docker build -t my-frontend ./frontend
   docker build -t my-backend ./backend

2. Initialize Docker Swarm:
   docker swarm init

3. Deploy Stack:
   docker stack deploy -c docker-compose.yml myapp

4. Verify Services:
   docker service ls

5. Access Applications:
   Frontend: http://localhost:8080
   Backend: http://localhost:5000


to doing Scaling (Docker Swarm)

1. to scale the backend service:
   docker service scale myapp_backend=3

2. to remove the stack:
   docker stack rm myapp

end;

