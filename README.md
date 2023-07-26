# Sprava - Enterprise Management Software Suite  🏢


Sprava is a proprietary software suite for enterprise management. The project is divided into two main parts: the frontend and the backend, developed using React and Django respectively.

## Project Structure  📂

The project is structured into two main directories:

- frontend/: Contains the source code for the frontend, developed in React.
- backend/: Contains the source code for the backend, developed in Django.

## Containerisation 🐳

We use Docker for service orchestration. A docker-compose.yml file is included in the project, which allows us to define and orchestrate three containers:

- The frontend container that serves the React application.
- The backend container that serves the Django API.
- An nginx container that serves as a reverse proxy.

The use of Docker ensures compatibility of dependencies and simplifies the development process. Furthermore, it allows Django and React to be started simultaneously for work on the project.

## Development Environment 💻

This repository is currently configured for development use only. It lacks certain necessary configurations for secure production deployment. Before attempting to use this in a production environment, please ensure proper production configuration files are added and all security measures are implemented.

## How to Start 🚀

To start the project, you will need Docker installed on your machine. Once Docker is installed, you can start the project by running the following command in the root directory of the project:

`docker-compose up --build`

This will build the necessary Docker images and start the containers. Once the containers are started, you can access the frontend application at `localhost:80` and the backend API at `localhost:80/api`.
