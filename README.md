# Node.js Container Project

This project is a simple Node.js application packaged in a Docker container. Below are the instructions to build and run the application.

## Prerequisites

- Docker installed on your machine.
- Node.js and npm (for local development).

## Project Structure

```
node-container-project
├── src
│   └── index.js
├── package.json
├── Dockerfile
└── README.md
```

## Getting Started

### Building the Docker Image

To build the Docker image, navigate to the project directory and run the following command:

```
docker build -t node-container-project .
```

### Running the Docker Container

After building the image, you can run the container using:

```
docker run -p 3000:3000 node-container-project
```

This will start the application and map port 3000 of the container to port 3000 on your host machine.

### Accessing the Application

Once the container is running, you can access the application by navigating to `http://localhost:3000` in your web browser.

## License

This project is licensed under the MIT License.