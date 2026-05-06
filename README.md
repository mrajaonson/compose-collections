# compose-collections

A curated collection of Docker Compose configurations for common services and stacks.

## Structure

```
compose-collections/
├── databases/       # Standalone database services (PostgreSQL, Redis, ...)
├── devtools/        # Developer tools (SonarQube, Gitea, ...)
├── monitoring/      # Monitoring & observability (Grafana, Prometheus, ...)
├── messaging/       # Message brokers (Kafka, RabbitMQ, ...)
└── stacks/          # Multi-service environments (LAMP, ELK, ...)
```

## Usage

Each service lives in its own folder and is self-contained.

```bash
cd databases/postgresql
cp .env.example .env
docker compose up -d
docker compose down -v
```
