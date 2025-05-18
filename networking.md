# Docker Networking

Networking allows containers to communicate with each other and with the host system. Containers run isolated from the host system and need a way to communicate with each other and with the host system.

By default, Docker provides two network drivers for us, the bridge and the overlay drivers.

docker network ls

NETWORK ID          NAME                DRIVER
xxxxxxxxxxxx        none                null
xxxxxxxxxxxx        host                host
xxxxxxxxxxxx        bridge              bridge

Key Concetps:

i. Bridge network is like a virtual LAN created by Docker.

ii. On the default bridge network, container can communicate with each other using IP adderess but can not uisng container name. 
   because container name is not resolvable on the default bridge network. for this we need to use user defined network.


## user define bridge

docker network create -d bridge bridge-test

attatch container to this bridge network.

docker network connect bridge-test container1

docker network connect bridge-test container2

docker exec -it container1 sh

ping container2







