# docker-cmd

### Get Images
```
docker images 
```

### Search Images
```
docker search node
```
### pull(install) Images ( it work for both run images or pull(download images if not exist )
```
docker pull node
```
##### docker pull <image-name>


### List all containers
```
docker ps 
```
```
docker ps -all or -a
```


### Create Container
```
docker run hello-world
```
 docker run <image-name>:tag  <br>
 tag is optional <br>
```
docker run --name hello-app hello-world or image-id
```
 --name custom container name  <br>

### To inspect the container 
```
docker inspect container-id
```


### run container in cmd (-it) gives access to a terminal or detach (-d) run in the background
```
docker run --name hello-app -d hello-world
```
```
docker run --name hello-app -it hello-world
```
### run container in cmd (-it) gives access to a terminal or detach (-d) run in the background
```
docker run --name hello-app -it -d hello-world
```
```
docker exec -it hello-app2
```
```
docker run --name hello-app3 -it hello-world
```
```
docker run --name hello-app3 -it --rm hello-world
```
temporary container after exit container will be deleted (for temporary use) <br>

docker exec -it hello-app2 ->(custom-container-name) <br>

### stop container 
```
docker stop hello-app4
```
hello-app4 -> container-name <br>

### start container 
```
docker start hello-app4
```
hello-app4 -> container-name <br>

### delete container 
```
docker rm hello-app4
```
hello-app4 -> container-name <br>

### docker remove the image 
```
docker rmi hello-world
```
hello-world -> image-name <br>

### docker remove all containers which inactive
```
docker container prune
```

### docker remove all containers and images and network
```
docker system prune
```

### docker container logs 
```
docker logs container-name
```

