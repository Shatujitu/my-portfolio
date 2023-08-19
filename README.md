# Portfolio Deployment Guide

### Postgres
```
docker compose -p portfolio --project-directory . -f postgres/docker-compose.yml build
```
```
docker compose -p portfolio --project-directory . -f postgres/docker-compose.yml up -d
```

### Strapi
```
docker compose -p portfolio --project-directory . -f strapi/docker-compose.yml build
```
```
docker compose -p portfolio --project-directory . -f strapi/docker-compose.yml up -d --scale strapi=2
```

### Traefik
```
cd traefik
```
```
docker compose -p portfolio -f docker-compose.yml build
```
```
docker compose -p portfolio -f docker-compose.yml up -d
```
