# An Introduction to Dockerization

- Docker is one such implementation of the idea of containerization

## What is Containerization?

- That is the idea behind containerization: putting your applications inside a self-contained package, making it portable and reproducible across various environments.

- Develop and run the application inside an isolated environment (known as a container) that matches your final deployment environment.

- Put your application inside a single file (known as an image) along with all its dependencies and necessary deployment configurations.

- Share that image through a central server (known as a registry) that is accessible by anyone with proper authorization.

## What is a Container?

- A container is sort-of like a virtual-machine without the overhead of the operating system of the virtual machine. Docker communicates with the main operating system of the computer to allocate necessary resources for the container.
- A container is an image in the running state.

## What is an Image?
- Images are multi-layered self-contained files that act as the template for creating containers. They are like a frozen, read-only copy of a container. Images can be exchanged through registries.
- Image formats have been standardized by the Open Container Initiative (OCI), which means an image built with docker can be used with other containerization engines.

## What is a registry?
- A registry is a platform for which docker images are uploaded and downloaded. Docker Hub and Quay are very popular ones.

- You can also create your own image registry for hosting private images.

## Container Creation and Starting

- `docker container ls --all` provides a list of all containers
- `docker container run <image-name>` which is in reality a combination of two separate commands. These commands are as follows:

- `docker container create <image-name>` command creates a container from a given image.
- `docker container start <container-identifier>` command starts a container that has been already created.
