# Docker
1. Build the Docker image
```shell
docker build -t my-postgresql-image .
```
2. Run without docker compose
```shell
docker run -d -p 5432:5432 --env-file /path/to/db.env --name my-postgresql-container my-postgresql-image
```


