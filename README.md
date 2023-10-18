# Skillfolio
 It combines the words "skills" and "portfolio" to represent a collection of your technical skills showcased in a CV format. It conveys the idea of presenting your abilities and accomplishments in a visually appealing and accessible manner.
# Docker
1. Run docker compose
```shell
docker-compose up
```
# WebServer
1. Nginx
```shell
sudo apt-get update
sudo apt-get install nginx
```
2. Add configuration file
```shell
touch /etc/nginx/conf.d/your-project.conf
```
3. Configure Reverse Proxy
```yaml
server {
    listen 80;
    server_name your-domain.com;

    location /api/ {
        proxy_pass http://localhost:8080; # Point to your Spring Boot backend
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
    }

    location / {
        root /path/to/your/frontend/files; # Specify the path to your Angular frontend
        index index.html;
    }
}
```
4. Test configuration
```shell
sudo nginx -t
```
5. Reload Nginx
```shell
sudo systemctl reload nginx
```
6. ##### DNS Configuration:
If your project is accessible via a domain name, make sure to configure your DNS settings to point to the server where Nginx is installed.

7. ##### Firewall and Security:
Review and configure your server's firewall settings to allow traffic on the Nginx ports (usually 80 and 443 for HTTP and HTTPS). Additionally, consider implementing security measures such as TLS/SSL encryption if your project handles sensitive data.

8. ##### Monitoring and Scaling:
Monitor the performance of your Nginx reverse proxy and consider implementing load balancing and caching if needed for scalability.
