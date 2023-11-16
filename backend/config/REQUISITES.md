# Requisites

### Local Git Repository - 1
```shell
cd ~; mkdir "server-config"; chmod 700 "server-config"; cd "server-config"; git init
```

### Using SSH Keys - 2
```shell
ssh-keygen -t rsa -b 4096 -C "your-email@example.com"
```

### Using GitHuv Access token - 3

#### Command Line Arguments:

You can pass properties as command-line arguments when starting the application.
Example: java -jar your-application.jar --property=value
Environment Variables:

#### Set environment variables to pass configuration to your application.
Example: export PROPERTY_NAME=value (Linux) or set PROPERTY_NAME=value (Windows)
Configuration Files:

#### Externalize configuration using property files (e.g., application.properties or application.yml).
You can have multiple property files for different environments.
Example: application-dev.properties or application-prod.properties
System Properties:

#### Use Java system properties to pass configuration.
Example: java -jar -Dproperty=value your-application.jar