# Some of the docker commands

## docker images 

List of dockerimages

## docker build

build image from docker

## docker run

runs a docker container from the image.

There are many arguments that we can use with the docker run command. Here are some of the most common ones:

docker run -d -> run container and print container id.

docker run -p -> maps a container port to a host port.

## docker ps || docker ps -a

lists of all the running containers. -a is used to list all the containers including the stopped ones.

## docker stop

stop running container

## docker start

start a stopped container.

## docker rm

removes a stopped container.

# docker pull

downloads an image from the docker hub.

# docker push

uploads an image to the configured registry.

## docker exec

run a commnd in a running container.

## docker logs <container-id>

view logs of a container

## docker inspect <container-id>

detail container info

