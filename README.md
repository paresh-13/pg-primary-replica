# Single-Primary PostgreSQL Replication with Docker-compose

Run primary and replica in background:
```bash
docker-compose up -d postgres_primary postgres_replica
```

Stop all services and remove volumes:
```bash
docker-compose down -v

Prerequisites
Before you begin, ensure you have met the following requirements:

Docker installed on your machine
Docker-compose installed


Starting the Services
Start the Docker containers using Docker-compose:

```bash
docker-compose up -d
This command will start up the necessary services defined in your docker-compose.yml file.

```bash
docker exec -it primary_db_container bash
Replace primary_db_container with the actual name of your primary database container.

```bash
psql -U myuser -d postgres
Connect to PostgreSQL primary

```bash
psql -U replicator -d postgres
#Connect to PostgreSQL replica
