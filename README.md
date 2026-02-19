---
title: "Despliegue de Servidor Web con Docker"
date: 2023-10-27
tags: ["Docker", "Linux", "Nginx"]
---

### Objetivo del Laboratorio
Configurar un entorno de microservicios usando Docker Compose para un servidor Nginx con persistencia de datos.

### Herramientas utilizadas
- **SO:** Ubuntu Server 22.04
- **Tecnología:** Docker v24.0.5
- **Redes:** Bridge network aislada

### Configuración del `docker-compose.yml`
```yaml
version: '3'
services:
  web:
    image: nginx:latest
    ports:
      - "80:80"
