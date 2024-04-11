# MERN CRUD Application with Docker and GitHub Actions

This project is a MERN (MongoDB, Express.js, React.js, Node.js) stack application for managing users (Create, Read, Update, Delete operations). The project is containerized using Docker, orchestrated using Docker Compose, and automated using GitHub Actions.

## Project Structure
 
The project consists of two main parts:

1. **Client**: A React.js application for the frontend.
2. **API**: A Node.js/Express.js application for the backend.

Both the client and the API have their own Dockerfiles for creating Docker images.

## Docker Compose

We use Docker Compose to manage and orchestrate our multi-container application. Docker Compose allows us to define our multi-container application with all of its dependencies in a single file, which simplifies the deployment process and ensures that our application runs the same way in every environment.

## GitHub Actions

We use GitHub Actions to automate the process of building and pushing our Docker images to Docker Hub. The workflow is triggered whenever you push to the `main` branch of your GitHub repository.

The workflow does the following:

1. Checks out your code.
2. Logs in to Docker Hub.
3. Sets up Docker buildx.
4. Builds and pushes the API Docker image.
5. Builds and pushes the Web Docker image.

Please replace the placeholders with your actual Docker Hub username and repository name as needed.

## Deployment to Docker Hub

Here are the steps to push your Docker images to Docker Hub:

1. Build your Docker images using `docker-compose build`.
2. Log in to Docker Hub using `docker login`.
3. Tag your images with your Docker Hub username and the repository name using `docker tag`.
4. Push your images to Docker Hub using `docker push`.

Please replace the placeholders with your actual Docker Hub username and repository name as needed.

Enjoy your journey with Docker, Docker Compose, GitHub Actions, and MERN stack!
