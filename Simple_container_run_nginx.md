## docker container run --publish 80:80 nginx

- Download nginx image from Docker Hub
- Start a new container with this image
- the **--publish** option opens the host port 80 and redirect to container`s 80 port
- if something is already running on port 80, it will give a "bind error", we can change left port (host port) to anything, for example: 8080:80

## docker container run --publish 80:80 --detach nginx

- The same above, but runs the container in the background.

## docker container ls -a

- show all containers, even the killed containers

## docker container run --publish 80:80 --detach --name webhost

- Run a ngix container in background, with the name host

## docker container logs webhost

- Show the logs of a specific container

## docker container top webhost

- show the process running inside one container

## docker container rm 97b

- let's say that the container ID of webhost is 97b82145a2e2
- we don't need the specify the whole id, only until it's unique, compared to others containers
