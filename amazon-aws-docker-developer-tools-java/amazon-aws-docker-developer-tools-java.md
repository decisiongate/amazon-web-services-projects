## Amazon AWS Docker developer tools & Java

## Technology stack
* Docker Hub
* Docker Engine
* Docker containers for the Amazon Elastic Compute Cloud (EC2)

[docker-developer-tools-java](https://github.com/docker/labs/tree/master/developer-tools/java/)
https://github.com/docker/labs/blob/master/developer-tools/java/chapters/ch08-aws.adoc

## Docker commands
- Checking the docker version:
docker -v OR docker --version
- Get currently running containers (only the active containers):
docker ps
- Get all containers ( all running + stopped):
docker ps -a
- Get a list of images available:
docker images
- Removing image:
docker rmi image-id
- Remove container:
docker container rm container-id
- Start/run a container:
docker run image-name
- Start the Stopped Container:
docker start container-id
- Stop running container:
docker stop container-id
- Get the last created container:
docker ps -l
- Go to the bash mode of the running container:
docker exec -it running-container-name bash
- Get IP Address of the docker container:
docker inspect container-id
- Display the disk usage of the docker:
docker system df
- See a list of volumes:
docker volume ls
- Remove a volume:
docker volume rm volume-name
- Prune volumes used by containers:
docker volume prune --force
- Prune volumes except labelled with the "keep" label:
docker volume prune --filter"label!=keep"
- Clean up any resources: images, containers, volumes, and networks that are not associated with a container:
docker system prune
- Additionally remove any stopped containers and all unused images:
docker system prune -a
