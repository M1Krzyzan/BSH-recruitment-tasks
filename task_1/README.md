# Hello World Docker Container

This repository contains a simple Docker container that prints "Hello World" by default. It also allows customization of the output using an environment variable.
## Prerequisites

Before running this project, make sure you have the following installed:

- [Docker](https://www.docker.com/) (Ensure Docker is running)

## Usage Instructions
### 1. Clone repository
```sh
git clone https://github.com/M1Krzyzan/BSH-recruitment-tasks
cd ./task_1
```
### 2. Build the Docker Image
Run the following command in the same directory as the `Dockerfile`:
```sh
docker build -t hello-world .
```

### 3. Run the Container
- Default behavior (prints `"Hello World"`):
  ```sh
  docker run hello-world
  ```
  
- Custom behavior (replace `"World"` with another word, e.g., `"Student"`):
  ```sh
  docker run -e NAME=Student hello-world
  ```
  Output:
  ```
  Hello Student
  ```