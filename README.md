# repotest1

Base Django project using Docker and MariaDB for development.

## Prerequisites

- Docker and Docker Compose installed.

## Setup

1. Build and start the containers:

   ```bash
   docker-compose up --build
   ```

2. Apply migrations:

   ```bash
   docker-compose run web python manage.py migrate
   ```

3. Create a superuser (optional):

   ```bash
   docker-compose run web python manage.py createsuperuser
   ```

The Django app is available at [http://localhost:8000](http://localhost:8000).
