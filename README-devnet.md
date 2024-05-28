# Masa Subtensor

This repository contains the Masa Subtensor Rust application that can be built and run using Docker. The Dockerfile is set up to compile the Rust application and execute a startup script.

## Prerequisites

Make sure you have Docker installed on your machine. You can download and install Docker from [here](https://www.docker.com/products/docker-desktop).

## Building the Docker Image

To build the Docker image using the `Dockerfile.masa`, run the following command in your terminal:

```sh
docker build -f Dockerfile.masa -t masa-subtensor .
```

This command tells Docker to use `Dockerfile.masa` to build the image and tag it as `masa-subtensor`.

## Running the Docker Container

To run the Docker container, use the following command:

```sh
docker run -it --rm masa-subtensor
```

This command starts a new container from the `masa-subtensor` image and runs it interactively. The `--rm` flag ensures that the container is removed after it stops.

## Summary of Commands

- **Build the Docker image:**
  ```sh
  docker build -f Dockerfile.masa -t masa-subtensor .
  ```

- **Run the Docker container:**
  ```sh
  docker run -it --rm masa-subtensor
  ```

## Additional Information

The Dockerfile installs necessary dependencies, builds the Rust application in release mode, and ensures the `localnet.sh` script is executable. It sets the entry point to run the `localnet.sh` script when the container starts.

If you encounter any issues or have questions, please refer to the Docker documentation or reach out to the repository maintainer.

---

This README provides basic instructions for building and running the Docker container for the Masa Subtensor Rust application. Make sure to update the README with any additional information specific to your application as needed.
