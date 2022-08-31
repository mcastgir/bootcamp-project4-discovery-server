# Project Discovery Server
> Microservice **Discovery Server** Bootcamp NTT Data

This project include:
- Spring Cloud Config
- Spring Cloud Eureka Server
- Spring Cloud Bootstrap
- Github Actions
- Docker

### Docker

1. Create Image Config Server in Docker
```  
docker build -t discovery-server .
```

2. Create Container

```
docker run -p 8761:8761 --name discovery-server-instance --link config-server-instance:latest -d discovery-server:latest
```

