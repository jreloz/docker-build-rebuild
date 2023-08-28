# docker-build-rebuild


### build docker
1. docker build -t tiosroadhouse-app .
2. docker run -d -p 8080:80 --name tiosroadhouse-api tiosroadhouse-app


### rebuild docker
1. docker build -t tiosroadhouse-app .
2. docker stop tiosroadhouse-api
3. docker rm tiosroadhouse-api
4. docker run -d -p 8080:80 --name tiosroadhouse-api tiosroadhouse-app
