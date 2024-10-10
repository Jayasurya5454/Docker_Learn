docker build -t jayasurya5454/node-task
# Docker Image Build and Push Instructions

This document provides instructions on how to build and push Docker images to Docker Hub.

## Prerequisites

- Ensure Docker is installed on your machine.
- Ensure you have a Docker Hub account.

## Steps

1. **Build Docker Images**

    Use the following commands to build your Docker images. Replace `jayasurya5454` with your Docker Hub username if different.

    ```bash
    docker build -t jayasurya5454/python-task:latest .
    docker build -t jayasurya5454/react-task:latest .
    ```

2. **Log in to Docker Hub**

    Log in to your Docker Hub account using the command below. You will be prompted to enter your Docker Hub username and password.

    ```bash
    docker login
    # provide credentials
    ```

3. **Push Docker Images to Docker Hub**

    Push the built images to Docker Hub using the following commands:

    ```bash
    docker push jayasurya5454/python-task:latest
    docker push jayasurya5454/react-task:latest
    ```

4. **Verify the Images on Docker Hub**

    After pushing the images, you can verify them on Docker Hub by logging into your Docker Hub account and navigating to the "Repositories" section. You should see your `python-task` and `react-task` images listed.

By following these steps, you will successfully build and push your Docker images to Docker Hub.
