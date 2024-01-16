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
    docker run -d -p 3000:5173 --name my-app docker-react:1.0
```