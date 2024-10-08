# Use the official Node.js image as the base image for the build stage
FROM node:16-alpine as build

# Set the working directory inside the container
WORKDIR /app

# Copy all files from the current directory to the working directory in the container
COPY . .

# Install dependencies
RUN npm install

# Build the React application
RUN npm run build

# Use the official Nginx image as the base image for the production stage
FROM nginx:alpine

# Copy the build output from the build stage to the Nginx HTML directory
COPY --from=build /app/build /usr/share/nginx/html

# Expose port 80 to the outside world
EXPOSE 80

# Start Nginx when the container starts
CMD ["nginx", "-g", "daemon off;"]
