# MinIO Docker Setup

This project sets up a MinIO server using Docker Compose.

## Prerequisites

- Docker
- Docker Compose

## Setup

1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Create a `.env` file in the root directory and add the following environment variables:
    ```env
    MINIO_ROOT_USER=your-root-user
    MINIO_ROOT_PASSWORD=your-root-password
    ```

3. Start the MinIO server:
    ```sh
    docker-compose up -d
    ```

## Usage

- Access the MinIO server at `http://localhost:9000`
- Access the MinIO console at `http://localhost:9001`

## Volumes

- The MinIO data is stored in `~/minio/data` on the host machine.

## Stopping the Server

To stop the MinIO server, run:
```sh
docker-compose down
