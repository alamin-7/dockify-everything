# Docker volumes

## Problem without volumes

It is very common to persist data in a container. When a container is deleted or restarted, all the data in the container is lost. 
To persist dada, we need to use volues.

## Solution

There are ways docker solve this problem.

1. Volues
2. Bind mounts

Volume create:

docker volume create <volume_name>

Now to mount the volume to a container:

docker run -it -v <volume_name>:/data <image_name> /bin/bash

This command will mount the volume to the /data directory in the container. Any data written to /data will be persisted in the volume 
on the host machine file system.

