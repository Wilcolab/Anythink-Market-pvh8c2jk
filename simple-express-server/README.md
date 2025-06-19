# Simple Express Server

This project is a simple Express server that listens on port 8001. It is designed to demonstrate the setup of an Express application with Docker and nodemon for automatic reloading during development.

## Project Structure

```
simple-express-server
├── src
│   └── server.js        # Entry point of the application
├── package.json         # Configuration file for npm
├── yarn.lock            # Dependency lock file
├── Dockerfile           # Instructions to build a Docker image
└── README.md            # Project documentation
```

## Getting Started

### Prerequisites

- Node.js (version 14 or higher)
- Yarn (package manager)
- Docker (for containerization)

### Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd simple-express-server
   ```

2. Install dependencies:
   ```
   yarn install
   ```

### Running the Server

To start the server with automatic reloading, use the following command:
```
yarn start
```

The server will be running at `http://localhost:8001`.

### Building the Docker Image

To build the Docker image, run:
```
docker build -t simple-express-server .
```

### Running the Docker Container

After building the image, you can run the container with:
```
docker run -p 8001:8001 simple-express-server
```

The server will be accessible at `http://localhost:8001`.

## License

This project is licensed under the MIT License.