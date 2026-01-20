# 🐳 Essential Docker Commands

## 📦 Containers

* **docker create `<image>`**: Creates a container from an image without starting it.
* **docker create --name `<name>` `<image>`**: Creates a container with a custom name.
* **docker run `<image>`**: Creates and starts a container from an image.
* **docker run -d `<image>`**: Runs a container in detached (background) mode.
* **docker run --name `<name>` -p `<host_port>`:`<container_port>` `<image>`**: Runs a container with a name and port mapping.
* **docker start `<container_id|name>`**: Starts a stopped container.
* **docker stop `<container_id|name>`**: Stops a running container gracefully.
* **docker restart `<container_id|name>`**: Restarts a container.
* **docker rm `<container_id|name>`**: Removes a stopped container.
* **docker rm -f `<container_id|name>`**: Forces removal of a running container (stop + remove).
* **docker ps**: Lists running containers.
* **docker ps -a**: Lists all containers, including stopped ones.
* **docker logs `<container_id|name>`**: Displays container logs.
* **docker logs -f `<container_id|name>`**: Follows container logs in real time.
* **docker exec -it `<container>` /bin/bash**: Opens an interactive Bash shell inside the container.
* **docker exec -it `<container>` sh**: Opens an interactive shell when Bash is not available.

## 🖼️ Images

* **docker images**: Lists images available on the host.
* **docker pull `<name>`:`<tag>`**: Downloads an image from a registry (default tag is latest).
* **docker image rm `<name>`:`<tag>`**: Removes a specific image.
* **docker rmi `<image_id>`**: Removes an image by ID.
* **docker build -t `<name>`:`<tag>` `<path>`**: Builds an image from a Dockerfile.
* **docker tag `<source>` `<target>`**: Creates a new tag for an image.
* **docker history `<image>`**: Shows the history and layers of an image.
* **docker inspect `<name|id>`**: Displays low-level information about containers or images.

## 📁 Volumes

* **docker volume ls**: Lists volumes.
* **docker volume create `<name>`**: Creates a new volume.
* **docker volume rm `<name>`**: Removes a volume.
* **docker volume inspect `<name>`**: Displays detailed information about a volume.
* **docker run -v `<volume>`:/path/in/container `<image>`**: Mounts a volume into a container.

## 🌐 Networks

* **docker network ls**: Lists available Docker networks.
* **docker network create `<name>`**: Creates a new network.
* **docker network rm `<name>`**: Removes a network.
* **docker network inspect `<name>`**: Displays detailed information about a network.
* **docker network connect `<network>` `<container>`**: Connects a container to a network.
* **docker network disconnect `<network>` `<container>`**: Disconnects a container from a network.

## 🛠️ Maintenance

* **docker stats**: Displays real-time CPU, memory, network, and I/O usage of containers.
* **docker system df**: Shows Docker disk usage.
* **docker system prune**: Removes unused containers, networks, and dangling images.
* **docker system prune -a**: Removes all unused containers, networks, and images (not just dangling ones).

## 🚀 Advanced commands

* **docker top `<container>`**: Displays running processes inside a container.
* **docker diff `<container>`**: Shows filesystem changes in a container.
* **docker cp `<container>`:`<src>` `<dest>`**: Copies files between container and host.
* **docker commit `<container>` `<image_name>`**: Creates a new image from a container’s changes.

## 🧩 Docker Compose

* **docker compose up**: Builds (if needed) and starts services defined in a compose file.
* **docker compose down**: Stops and removes containers, networks, and volumes created by up.
* **docker compose build**: Builds or rebuilds services.
* **docker compose logs**: Displays logs for services.
* **docker compose logs -f**: Follows logs for all services.
* **docker compose ps**: Lists containers for the services.

---

✨ *Quick reference Docker cheat sheet, aligned with official Docker documentation.*
