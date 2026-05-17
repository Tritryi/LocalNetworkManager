# LocalNetworkManager
The goal of this project is to train myself in system administration using local docker service. I created a complex local network that is easily manageable and can be customized quickly.

The main component of this project is the file `docker-compose.yml` it will create all the local network with desired images and configuration.

# The network
This is the composition of the current network.

- pihole : pihole container. Allows us to replace our local dns and create "fake" domain names.

- mywebserv : a simple web server using Apache official image.

- nginx-proxy : a nginx container used as a reverse proxy. Only nginx and pihole have an actual port binding, the other services are redirected using this nginx container.

- dozzle : a docker management web interface.

- networkpi : the bridge network that links all the containers.


# Project structure

