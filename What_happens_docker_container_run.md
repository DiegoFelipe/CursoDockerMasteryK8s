1. Looks for that image locally in image cache
2. If it doesn't find, it goes to Docker Hub
3. Downloads the latest version
4. Created a new container based on that image and prepares to start
5. Give a network to the container
6. open up port 80
7. starts container by using the CMD in the image DockerFile