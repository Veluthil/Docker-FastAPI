# Dockerized FastAPI Application

This repository contains a basic FastAPI application that is containerized using Docker for easy deployment and execution in any environment.

## Requirements

- Docker
- Internet connection (for pulling Docker images)

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/Veluthil/Docker-FastAPI.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Docker-FastAPI
   ```

3. Build the Docker image (you can call it however you like):

   ```bash
   docker build -t fastapi-app .
   ```

   This will build the Docker image based on the provided Dockerfile.

4. Run the Docker container:

   ```bash
   docker run -d -p 8000:8000 fastapi-app
   ```

   This will start the FastAPI application inside the Docker container and map port 8000 on the host to port 8000 inside the container.

5. Access the application:

   Open your web browser and go to [http://localhost:8000](http://localhost:8000). You should see the FastAPI application running.

## Customization

If you want to modify the FastAPI application or add additional functionality, you can do so by editing the `main.py` file. The current application provides a basic "Hello, World!" response, and you can extend it to suit your needs.

## API Documentation

The FastAPI application automatically generates interactive API documentation using Swagger UI. You can access the API documentation by visiting [http://localhost:8000/docs](http://localhost:8000/docs) in your web browser. It provides details about the available endpoints, request/response schemas, and allows you to interact with the API.

## Acknowledgements

- This project utilizes the FastAPI framework: [https://fastapi.tiangolo.com/](https://fastapi.tiangolo.com/)
- Docker: [https://www.docker.com/](https://www.docker.com/)
