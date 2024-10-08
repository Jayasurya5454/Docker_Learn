
## Installing Docker on Linux

To install Docker on a Linux system, follow these steps:

1. **Update your package index and install Docker:**
    ```sh
    sudo apt update && sudo apt install docker-ce containerd.io docker-ce-cli
    ```

2. **Verify the Docker installation:**
    ```sh
    docker --version
    ```

3. **Run a test Docker image:**
    ```sh
    docker run hello-world
    ```

4. **Check running Docker processes:**
    ```sh
    docker ps
    ```

5. **List all Docker containers (including stopped ones):**
    ```sh
    docker ps -a
    ```
