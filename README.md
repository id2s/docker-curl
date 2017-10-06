# docker-curl [![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](LICENSE) [![Docker Automated buil](https://img.shields.io/docker/automated/jrottenberg/ffmpeg.svg)](https://hub.docker.com/r/id2s/docker-curl/)

Docker image for Debian Jessie with curl preinstalled

## Installation

- [Install Docker](https://docs.docker.com/engine/installation/)
- Run docker commnad to get an image: `docker pull id2s/docker-curl:latest`
- Validate image successfully downloaded: `docker images`

## Run 

Start a **mysql** server instance:
    
    # General form
    $ $ docker run [OPTIONS] IMAGE[:TAG|@DIGEST] [COMMAND] [ARG...]
    
    # Example
    $ docker run -d --name curl id2s/docker-curl:latest

Other **commands**:

    # Kill the container
    docker kill [container-id]
    
    # Shell script/shell access
    $ docker exec -it curl bash
    
    # Viewing MySQL logs
    $ docker logs curl
    
    # Start exisitng container (often: after Docker Engine update)
    docker start [CONTAINER ID]