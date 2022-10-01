# Project2-Compose
Project2-Compose
## Docker-In-Docker container
Docker-in-Docker(dind) container will be listening on port 2376 
## Jenkin container
A Jenkin container which uses the dind container to run a Jenkin pipeline. 
We will be able to reach Docker-in-Docker container from Jenkins on tcp://docker:2376.m('docker' is the the alias of network 'jenkins')
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
