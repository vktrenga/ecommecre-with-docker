# ecommerce-api

## Prerequisites

- [Install Docker](https://docs.docker.com/get-docker/)
- [Install Docker Compose](https://docs.docker.com/compose/install/)

## Docker Compose Setup

1. **Clone the repository**  
   ```sh
   git clone <your-repo-url>
   cd ecommecre-with-docker
   ```

2. **Build and start containers**  
   ```sh
   docker-compose up --build
   ```

   This will start both the API and MongoDB containers as defined in [docker-compose.yml](docker-compose.yml).

3. **Access the API**  
   The API will be available at [http://localhost:4000](http://localhost:4000).

## Common Docker Commands

- **Build Docker Image**
  ```sh
  docker build --tag <ImageName> .
  ```
  Example:
  ```sh
  docker build --tag e-commerce-api .
  ```

- **List Docker Images**
  ```sh
  docker images
  ```

- **Run Docker Image**
  ```sh
  docker run <ImageName>
  ```
  Example:
  ```sh
  docker run e-commerce-api
  ```

- **Run Docker Image with Port Mapping**
  ```sh
  docker run --publish 8000:8000 <ImageName>
  ```
  Example:
  ```sh
  docker run --publish 4000:8000 node-docker
  ```

  - `4000` is the Docker host port
  - `8000` is the application container port

## Notes

- For environment variables, see [.sample.env](.sample.env).
- The API source code is