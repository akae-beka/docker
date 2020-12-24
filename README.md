# docker
Main day-to-day docker knowledge

### docker info
_Display system-wide information_
```
docker info
```

### docker login
_Log in to a Docker registry_
```
docker login
```

### docker build
_Build an image from a_ __`Dockerfile`__

Build with tag latest
```
docker build -t swagger .
```

Build with the repository name and the latest tag
```
docker build -t datteops/swagger .
```

Build with the name of the repository and with the v1.0 tag
```
docker build -t datteops/swagger:v1.0 .
```

### docker images
_List images_
```
docker images
```

### docker run
_Run a command in a new container_
```
docker run -d -p 8080:8080 --name service-swagger datteops/swagger:v1.0
```

### docker ps 
_List containers_

List only containers running
```
docker ps
```

List all containers running and stopped
```
docker ps -a
```

### docker stop
_Stop one or more running containers_

Stop with container name
```
docker stop service-swagger
```

Stop with container ID
```
docker stop 52c2d69953a9
```

### docker start
_Start one or more stopped containers_

Start with container nome
```
docker start service-swagger
```

Start with container ID
```
docker start 52c2d69953a9
```

### docker logs
_Fetch the logs of a container_

Get logs with container name
```
docker logs service-swagger
```

Get logs with container ID
```
docker logs 52c2d69953a9
```

### docker rm
_Remove one or more containers_

First stop the container and remove only one container by name
```
docker rm service-swagger
```

remove only one container by ID
```
docker rm 662c38240042
```

### docker stats
_Display a live stream of containers resource usage statistics_
```
docker stats
```
