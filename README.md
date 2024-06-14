# Node.js Docker Application

## Description

This project demonstrates how to containerize a simple Node.js application using Docker. The application uses Express.js to serve a "Hello World" message.

## Prerequisites

- Docker installed on your machine
- Node.js installed on your machine (for local development)

## Setup

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/node-docker-app.git
    cd node-docker-app
    ```

2. Build the Docker image:
    ```sh
    docker build -t node-docker-app .
    ```

3. Run the Docker container:
    ```sh
    docker run -p 3000:3000 node-docker-app
    ```

4. Access the application in your browser at `http://localhost:3000`.

## Using Docker Compose

Alternatively, you can use Docker Compose to build and run the application:

1. Start the application using Docker Compose:
    ```sh
    docker-compose up
    ```

2. Access the application in your browser at `http://localhost:3000`.

## Project Structure

- `app.js`: The main application file
- `package.json`: Project metadata and dependencies
- `Dockerfile`: Instructions to build the Docker image
- `docker-compose.yml`: Docker Compose configuration file
- `.dockerignore`: Specifies files and directories to be ignored in the Docker build

## License

This project is licensed under the MIT License.
