# edProjects

## Microservices Architecture

This project implements a microservices architecture using Docker Compose. It includes a reverse proxy for routing
requests to different services, PostgreSQL for database management, and Redis for caching and others.

## Features:

- Docker Compose version: 3.9
- Reverse proxy: NGINX 1.25.5
- Database: PostgreSQL 16.3
- Redis 7.2.5

## Installation

1. Clone the repository
    ```bash
    git clone https://github.com/edonssfall/edDeplyment.git
    ```
2. Enter the project directory
    ```bash
    cd edDeplyment
    ```
3. Edit the `.env` file and set the environment variables
    ```bash
    cp envs-example/auth-django.env.example envs/auth-django.env
   cp envs-example/chats-react-ui.env.example envs/chats-react-ui.env
   cp envs-example/django.env.example envs/django.env
   cp envs-example/main-angular-ui.env.example envs/main-angular-ui.env
   cp envs-example/postgresSQL.env.example envs/postgresSQL.env
   cp envs-example/websockets-django.env.example envs/websockets-django.env
    ```
   
## Usage
Start the services using Docker Compose
```bash
docker-compose up
```

## Services
The project consists of the following services:

- Reverse Proxy (NGINX): Handles routing of requests to different services.
- PostgreSQL: Database management system.
- Redis: In-memory data structure store used for caching.
- Django: Auth service.
- Django: Websockets service.
- Angular: Main UI service.
- React: Chats UI service.