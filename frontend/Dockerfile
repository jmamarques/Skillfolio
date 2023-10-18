# Use an official Node.js runtime as a parent image
FROM node:14

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the application code into the container
COPY . .

# Build the Angular app for production
RUN ng build --prod

# Expose the port that the Angular app will run on
EXPOSE 4200

# Start the Angular app
CMD ["ng", "serve", "--host", "0.0.0.0", "--port", "4200"]
