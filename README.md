# Project2-Compose
Project2-Compose
## Docker-In-Docker container
Docker-in-Docker container will be listening on port 2376 
and since we gave it the network alias of docker then 
## Jenkin container
we will be able to reach Docker-in-Docker container from Jenkins on tcp://docker:2376.('docker' is the the network alias of  network 'jenkins')
## How to start/stop?
```
docker-compose up -d
docker-compose down
```
### Check the Jenkins container's log
```
docker logs project2-compose_jenkins_1
```
### Connect to the Docker-In-Docker container 
```
docker exec -it project2-compose_docker-in-docker_1 sh
```
