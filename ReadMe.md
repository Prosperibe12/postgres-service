# MongoDB Service

This repository contains PostgresDB service for a microservices application. The PostgresDB service runs a single instance of Postgres and is used primarily by the Authentication service for user management. For more information about the main project, visit [pdf2podcast-microservice](https://github.com/Prosperibe12/pdf2podcast-microservice).

## Installation

To install the PostgresDB service, follow these steps:

1. Clone the repository:
    ```bash
    https://github.com/Prosperibe12/postgres-service.git
    ```
2. Navigate to the project directory:
    ```bash
    cd postgres-service
    ```

## Usage

Apply the Kubernetes manifests to deploy PostgresDB:
Ensure you have a kubernetes cluster running
```bash
kubectl apply -f manifests
```
This will create the following resources:

A Single PostgresDB Instance.

A Service to expose PostgresDB internally.

A PersistentVolumeClaim (PVC) for data persistence.