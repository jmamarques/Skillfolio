# Use the official PostgreSQL image from Docker Hub
FROM postgres:13

# Set environment variables (adjust as needed)
ENV POSTGRES_USER=myuser
ENV POSTGRES_PASSWORD=mypassword
ENV POSTGRES_DB=mydb

# Copy initialization scripts to the container (if needed)
COPY init.sql /docker-entrypoint-initdb.d/

# Expose the default PostgreSQL port
EXPOSE 5432
