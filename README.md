# CI/CD Toolsets with asdf-vm Docker Images

This repository contains Dockerfiles and configurations for creating Docker images that are based on the custom [asdf-vm](https://github.com/jrosco/docker-container-asdf) version manager image. 

These images are designed to make it easier to manage and use multiple versions of different tools and programming languages within Docker containers. Additionally, this repository includes Dockerfiles for various tools, including AWS CLI, Helm, and Terraform. These Dockerfiles can be used to build Docker images for these tools, which can then be used in various environments to ensure consistency and reproducibility.


## Tools Included
- [terraform/open-tofo](terraform/) and tools
- [helm](helm/) and tools
- [browser-testing](browser-testing) and tools

## Prerequisites
- Docker with `docker-compose` support

## Usage

Run the below commands inside the toolset directoires e.g [terraform](terraform/)

### Build the Docker Image
To build the Docker image, run:
```sh
docker compose build
```

### Run the Docker Container
To run the Docker container, execute:
```sh
docker compose run toolset
```

## Configuration
The tools and their versions are managed using `asdf` and the `.tool-versions` file. Adjust the versions as needed.
