# devbox-remote

A project template with Devbox + DevContainer + DinD + Minikube configurations.

## Developer Guide

### Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

Or, you can use the [GitHub Codespaces](https://github.com/codespaces) instead of Visual Studio Code running on your local machine.

### Adding new dependencies to the development environment

You may use `devbox add` command to add pkgs from `https://www.nixhub.io/`.  
Or, checkout `taskfiles/_env.yml` and make changes as needed.

### Running Containers

**Docker** should be already up and running. You may use `docker` or `docker-compose` commands to manage the containers.

**Minikube** can be started using `task k8s:up` command. This will start a minikube cluster and create tunnel to access the services with type `LoadBalancer`.
