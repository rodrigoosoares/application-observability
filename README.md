# Spring application API with Prometheus and Grafana integration

## How to run it

### 1. Run containers
```bash
docker-compose up -f /env/docker-compose.yml
```

### 2. Execute Spring Boot application
```bash
mvn spring-boot:run
```
### 3. Access grafana endpoint
Access endpoint: ```localhost:3000```

Default login:
- **username**: admin
- **password**: admin

### 4. In grafana interface
- Go to **Data Sources** configuration
- Choose Prometheus data source
- Setup with Prometheus URL
  - In this case we are using the prometheus:9090, since we're using docker
