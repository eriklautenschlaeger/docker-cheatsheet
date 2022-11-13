# Docker

## Cheat Sheet
### Show list of running containers 
`docker ps`

### Show list of all containers 
`docker ps -a`

### Start Container
`docker start <image_name>`

### Stop Container
`docker stop <image_name>`

### Delete Container
`docker rm <container_name>`

### Show list of all images
`docker images`

### Download Image
`docker pull <image_name>`

### Delete Image
`docker rmi <image_name>`

### Start new Container from an Image (pull + start)
`docker run <image_name>`

### List all networks
`docker network ls`

### Create new Network
`docker network create <network-name>`

### Start new specifically named, detached Container from an Image using a tag and port mapping
`docker run -d -p <hostport>:<containerport> --name <containername> <container>:<tag>`

### Another example of a more complex run command in a different syntax
```
docker run -d \
-p <hostport>:<containerport> \
-e <ENVIRONMENT_VARIABLE>=<value> \
--name <containername> \
--net <network-name> \
<container>:<tag>
```

