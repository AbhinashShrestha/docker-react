# docker-react

## How to build the image
``` bash 
    docker build -t docker-react:1.0 .
```
You will have a image named docker-react
which you can check by running 
```
docker ps
```

## How to use the image

``` bash
docker run -d -p 3000:5173 -v "$(pwd):/app" -v  /app/node_modules  --name my-app docker-react:1.0
```
this command will start a new Docker container in the background from the docker-react:1.0 image you just built, map port 5173 in the container to port 3000 on the host, mount the current directory to /app in the container, create a volume for /app/node_modules, and name the container my-app. The application inside the Docker container would then be accessible on port 3000 of the host machine.

Then go to localhost:3000
