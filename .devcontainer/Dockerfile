# .devcontainer/Dockerfile
FROM mcr.microsoft.com/vscode/devcontainers/cpp:0-ubuntu-22.04

# Install additional packages
RUN apt-get update \
    && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
        valgrind \
        neofetch \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Create a folder named "CartellaContainer"
RUN mkdir /CartellaContainer

# Set the working directory to /CartellaContainer
WORKDIR /CartellaContainer
