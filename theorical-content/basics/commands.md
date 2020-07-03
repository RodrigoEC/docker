# Docker commands

## Index

## Introduction

I'm gonna break this commands into 

## Basics:

### __Docker pull <image-name>__

This command downloads a container image with the same "image-name" that
as set.

Docker images can be found at [Docker hub](https://hub.docker.com/).

__Example:__ Pull of the ubuntu's image

```Docker 

Docker pull ubuntu

```

![Docker pull ubuntu](/img/docker_pull.png)


> :warning: Attention: If you want to download a image that is not labeled
as `official` there's a little difference in the command:

__Example:__ Pull of a image created by the user douglasq.
```Docker
Docker pull douglasq/alura_books
```


### __Docker run <image-name>__

This command runs the image that is passed as parameter, if the image name is not found locally the docker tries to find it on the [docker hub/ docker store](https://hub.docker.com/). 

Once the image is found the docker engine create and run the container. 

Example: Creating a "hello-world" container
```
docker run hello-world
``` 

![Docker run command](/img/dockerRun.png)

### __Docker images__

Displays all the images that were pulled or created locally containing
the following information:

- __REPOSITORY:__ Image's name;
- __TAG:__ Version of the image. Lastest means that it is the more recent version
- __IMAGE ID:__ Image identifiar;
- __CREATED:__ When the image was created locally;
- __SIZE:__ The size of image file.

![Docker image](/img/docker_images.png)



### **Docker ps/ docker ps -a**

The `docker ps` shows us the containers that are active in the moment. In the other hand the `docker ps -a` command shows us all the containers create, active or not.

![docker ps -a command](/img/deactivedContainers.png)