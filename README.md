# Random Coffee-Mate & Order Roulette (RCMOR)

This repository contains a skeleton implementation of the Random Coffee-Mate & Order Roulette platform. It includes several Spring Boot microservices and a Vite React frontend. Services are wired together using `docker-compose` and use PostgreSQL for persistence.

## Structure

- `api-gateway` – entry point for the frontend
- `user-service` – manage users and preferences
- `matchmaking-service` – schedule random coffee matches
- `order-service` – manage beverage orders
- `notification-service` – send notifications
- `analytics-service` – optional analytics module
- `frontend` – React/TypeScript client

## Running the stack

Build and start all services using Docker Compose. A helper script `run.sh` is provided so you can bring the stack up with a single command:

```bash
./run.sh
```

Each service exposes a basic `/actuator/health` endpoint and listens on ports 8080–8085. PostgreSQL runs on port 5432.

This is an early skeleton to demonstrate project layout. Business logic and API endpoints need to be implemented according to the requirements.
