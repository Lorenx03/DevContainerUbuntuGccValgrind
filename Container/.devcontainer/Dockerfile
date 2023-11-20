FROM --platform=linux/amd64 mcr.microsoft.com/devcontainers/cpp:1-ubuntu-22.04

# Install additional packages
RUN apt-get update \
    && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
        valgrind \
        neofetch \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*


# Se si vuole utilizzare una cartella nel container 
#RUN mkdir /CartellaContainer \
#    && chmod 777 /CartellaContainer

#WORKDIR /CartellaContainer


# Per sincronizzare i contenuti della cartella nel container con la cartella dell'host esegure questo comando
# find /workspaces -type d -name "Container" -exec rsync -a /CartellaContainer {} \;