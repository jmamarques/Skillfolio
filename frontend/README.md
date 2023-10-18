# Docker
1. Build the Docker image
```shell
docker build -t your-frontend-image . 
```
2. Run without docker compose
```shell
docker run -d -p 8081:4200 your-frontend-image
```