# docker-build-rebuild


# Example:
1. image_name = app_api
2. container_name = wneth_app


### build docker
1. docker build -t <image_name> .
2. docker run -d -p 8080:80 --name <container_name> <image_name>


### rebuild docker
1. docker build -t <image_name> .
2. docker stop <container_name>
3. docker rm <container_name>
4. docker run -d -p 8080:80 --name <container_name> <image_name>
