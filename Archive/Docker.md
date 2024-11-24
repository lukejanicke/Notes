# Docker

- [Docker](https://www.docker.com)

## Installation

Download and install **Docker Desktop** directly from the official website.

## Usage

Browse and search for images in the Docker app.

Pull an image using the app or the `docker pull` Command in Terminal.

```zsh
docker pull image/image:latest
```

Create and run a Docker container from an image with an interactive Bash shell. The current directory is mounted as `/workdir` in the container. Optionally, replace `$PWD` with a specific directory, like `~/Documents/Project`.

```zsh
docker run -it --name container_name -v $PWD:/workdir image_nameSpace/image_name:tag bash
```

### Terminal commands

| Command                               | Description                                      |
| ------------------------------------- | ------------------------------------------------ |
| `exit`                                | Exit the interactive shell.                      |
| `docker exec -it container_name bash` | Restart the interactive shell.                   |
| `docker stop container_name`          | Stop the container.                              |
| `docker start container_name`         | Restart the container.                           |
| `docker start -ai container_name`     | Restart the container with an interactive shell. |
| `docker rm container_name`            | Remove the container.                            |

> [!tip] Stop unused containers
> Remember to stop containers when they are not in use.
