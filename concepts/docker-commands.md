# Docker commands

## Index

## Introduction

I'm gonna break this commands into 

## Basics:

### **Docker run <image-name>**

This command runs the image that is passed as parameter, if the image name is not found locally the docker tries to find it on the [docker hub/ docker store](https://hub.docker.com/). 

Once the image is found the docker engine create and run the container. 

Example: Creating a "hello-world" container
```
docker run hello-world
``` 

![Docker run command](/img/dockerRun.png)

### **Docker ps/ docker ps -a**

The `docker ps` shows us the containers that are active in the moment. In the other hand the `docker ps -a` command shows us all the containers create, active or not.

![docker ps -a command](/img/deactivedContainers.png)