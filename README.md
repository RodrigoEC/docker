# :whale: Docker

The goal of this repository is for me to learn how to use Docker and Docker Compose.

## What is docker?

Click on the following link to know more about docker: [About docker](./concepts/aboutDocker.md). 

## Installing docker

[Docker's site](https://www.docker.com/products/docker-desktop)

### For windows:

There are two types of docker available for windows:

#### Docker for windows:

#### Docker for MacOS:

#### Docker for ubuntu:

Open your terminal and type the following commands

1. Before installing anything remove possible older docker versions:

    ```
    sudo apt-get remove docker docker-engine docker.io
    ```

2. Update your system's packages
    ```
    sudo apt-get update
    ```
3.  Add the docker repository official GPG key to the system
    ```
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
    ```

4. The following command adds the repository to the list of places the system goes to look for software
    ```
    sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
   ```

5. Update the packages information from all configured sources, once you do that you'll be able to acess the docker packages:
    ```
    sudo apt-get update
    ```

6. Finally install docker
    ```
    sudo apt-get install docker-ce 
    ```

To be sure that docker was install check the docker version by typing this following command:
    ```
    sudo docker version
    ```