# CONTAINERIZATION AND CREATING A FULL-STACK APP WITH DOCKER

## Docker Introduction

Docker is an open-source platform that automates the deployment, scaling and management of applications inside containers. Containers are lightweight, portable, and consistent environments that package an application with all its dependencies and environment settings [1].

### Importance of Docker in Software Development

Docker is crucial for modern software development for several reasons:

- It ensures the application runs consistently across development, testing, and production environments.
- Docker enhances portability, allowing workloads to run seamlessly across various environments including local developer laptops, physical or virtual machines in data centers, cloud providers, or a hybrid of these environments.
- Its lightweight and fast nature make Docker a cost-effective alternative to hypervisor-based virtual machines.
- Docker streamlines the development lifecycle by enabling developers to work in standardized environments using local containers [1]. This includes:
  -- Writing code locally and sharing it using Docker containers.
  -- Pushing applications into a test environment where automated and manual tests are run.
  -- Fixing bugs.
  -- Straightforward deployment of fixes to customers.

### Commands Used

Docker commands for Challenge 1 & 2:
| Commands | Use |
| --- | --- |
| docker build -t [image name] . | Builds and creates an image from a Dockerfile with the name ‘challenge1_image’ |
| docker images | Lists all the Docker images that are stored on local system. |
| docker ps | Lists all the running Docker containers on the system. |
| docker run | Runs a container from an image |
| docker stop | Stops a running container |
| docker rm | Removes a container |
| docker rmi | Removes an image |
| docker run -p 8080:80 [image name] | Runs a Docker container from a specified image and map ports between the host machine and the container. |

### Installation Steps

Install Docker on your system by following these steps:

- Docker Desktop can be installed on Windows, Mac and Linux. In my case, I’m using Windows OS.
- Before installation, ensure that your system meets the necessary requirements by checking the https://docs.docker.com/desktop/install/windows-install/
- Go to https://www.docker.com/products/docker-desktop/ and download the installer for Windows or MAC if you're using MAC.
- Go to your downloads folder, run the Docker Desktop Installer.exe

## CHALLENGE 1 & 2 SIMPLE STATIC PAGE SERVER & NODEJS APPLICATION

This section provides a basic introduction to using Docker for serving static pages. It includes creating a Dockerfile to expose endpoints for external clients and a Docker Compose file to orchestrate both the web server and the application.

## CHALLENGE 3 & 4 CREATING A FULL-STACK APPLICATION & SCALING UP AN APPLICATION

This section focuses on creating a complete application using Docker Compose, which brings together a web server (Nginx), an application service (Node.js), and a database (MariaDB). It also builds on the previous challenge by looking at how to scale the application to handle more users and traffic.
