# Docker-Hello-World
To get started with Docker and run a basic "Hello World" example, follow these steps:

### 1. **Install Docker**
   - **Linux:** You can install Docker using the package manager for your Linux distribution (e.g., `apt` for Ubuntu, `yum` for CentOS).
   - **Windows/Mac:** Download and install Docker Desktop from [Docker's official website](https://www.docker.com/products/docker-desktop).

### 2. **Verify Docker Installation**
   Open a terminal or command prompt and run the following command to check if Docker is installed and running:

   ```bash
   docker --version
   ```

   You should see the version of Docker that is installed.

### 3. **Run the Docker "Hello World" Container**
   To run a simple Docker container that prints "Hello World," execute the following command:

   ```bash
   docker run hello-world
   ```

   This command does the following:
   - **Pulls** the `hello-world` image from Docker Hub if it’s not already present on your system.
   - **Creates** a new container from this image.
   - **Executes** the container, which prints a "Hello from Docker!" message.

### 4. **Understanding the Output**
   The output will include a message like this:

   ```plaintext
   Hello from Docker!
   This message shows that your installation appears to be working correctly.
   ```

   The rest of the message will explain a bit about how Docker works and how the container was created and run.

### 5. **View Running Containers**
   To see the list of currently running containers, use:

   ```bash
   docker ps
   ```

   Since the `hello-world` container exits after printing the message, you won’t see it here.

### 6. **View All Containers (Including Stopped Ones)**
   To see all containers, including those that have stopped:

   ```bash
   docker ps -a
   ```

   This will list all containers, showing that the `hello-world` container ran and then exited.

### 7. **Remove the Container**
   If you want to remove the stopped container:

   ```bash
   docker rm [container_id]
   ```

   Replace `[container_id]` with the actual ID of the container, which you can find using the `docker ps -a` command.

This simple "Hello World" example shows how easy it is to use Docker to run isolated applications within containers.