# docker-minecraft

A nice and easy way to get a Minecraft server up and running using docker. For
help on getting started with docker see the [official getting started guide][0].
For more information on Minecraft and check out it's [website][1].

This repository is a fork from https://github.com/overshard/docker-minecraft

## Running this image

Running this will build you a docker image with the latest version of both
docker-minecraft and Minecraft itself. 

    git clone https://github.com/nicemd/docker-minecraft
    cd docker-minecraft
    docker-compose up

The Docker image is built on your computer and not downloaded from Docker hub.

## Running this image in a Docker Swarm

Only one swarm replica of the server is supported.


    git clone https://github.com/nicemd/docker-minecraft
    cd docker-minecraft
    docker stack deploy -c docker-compose.yml minecraft

## Minecraft Data directory

Your Minecraft world data will be placed in the `data` directory.

[0]: http://www.docker.io/gettingstarted/
[1]: http://minecraft.net/
