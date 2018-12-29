# docker-examples
This repository contains wide variety of Docker examples and scenarios

## Docker commands

* `docker build .` - to build the image with same context
* `docker build -f <docker file path> .` - to build with different docker file name other than Dockerfile
* `docker build -t <dockerid/containername> .` - to tag the image
* `docker run <containerid/tag image>` - to the run the docker image
* `docker run -p "inport:outport" <containerid/tag image>` - to run the image with speciifc port
* `docker run <containerid/tag image> bash` - to override the startup command. Eg: bash here

## Docker-compose commands

* `docker-compose up` - to start the container
* `docker-compose up --build` - to rebuild and start the app
* `docker-compose ps` - to list all the containers
* `docker-compose down` - to stop the containers

## Docker volume commands

* `docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app <dockerid/containername>` - in this case use workdir volumes for node modules and current working directoty for other files.
