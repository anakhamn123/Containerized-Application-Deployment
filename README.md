
# Containerized Application Deployment and Management Using Docker

## 1. Project Overview

This project demonstrates how to develop, containerize, deploy, and manage a Python Flask web application using Docker.

The application provides a web dashboard displaying project information, container details, deployment information, and technologies used.

## 2. Project Objectives

- Understand Docker containerization.
- Build and manage Docker images.
- Deploy a Flask application inside a Docker container.
- Use Gunicorn as a production application server.
- Manage containers using Docker Compose.
- Improve container security using a non-root user.
- Monitor application health using Docker health checks.

## 3. Technologies Used

- Python
- Flask
- Docker
- Docker Compose
- Gunicorn
- HTML
- CSS

## 4. Project Structure

```text
docker-project/
│
├── app.py
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── .dockerignore
├── README.md
│
├── templates/
│   └── index.html
│
└── static/
    └── style.css
```

## 5. Application Features

- Professional web dashboard.
- Flask-based web application.
- Docker containerization.
- Gunicorn application server.
- Non-root container user.
- Docker Compose management.
- Automated health checks.

## 6. Installation Requirements

- Python
- Docker Desktop
- Visual Studio Code
- Git (optional)

## 7. Build and Run the Application

Open the project folder in the terminal and run:

```bash
docker compose up -d --build
```

## 8. Verify the Application

Check container status:

```bash
docker compose ps
```

View application logs:

```bash
docker compose logs
```

Check the running container user:

```bash
docker exec my-container whoami
```

## 9. Access the Application

Open the following address in a web browser:

http://localhost:5000

Health-check endpoint:

http://localhost:5000/health

Expected health response:

```json
{
  "application": "Docker Flask Application",
  "status": "healthy"
}
```

## 10. Stop the Application

Run:

```bash
docker compose down
```

## 11. Conclusion

This project demonstrates the practical implementation of Docker-based application deployment and management.

It provides hands-on experience with containerization, application serving, security practices, container management using Docker Compose, and application health monitoring.
