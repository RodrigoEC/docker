# About Docker! 

## Index

- [Introduction](#introduction)
    - [The problem with physical servers](The-problem-with-Physical-Servers)
    - [The problem with Virtual Machines](The-problem-with-Virtual-machines)
        - [Advantages](#advantages)
        - [Desadvantages](#desadvantages)
- [Docker?](#docker)
    - [Containers](#containers)    
        - [advantanges](#advantages-container)
    - [Why use containers instead of the computer by itself?](#Why-use-containers-instead-of-the-computer-by-itself?)

## Introduction

Before we head to the definition of docker and it's tools I thinks it's important for us to understand why using docker and docker-compose is way better than using `physical servers` or `Virtual machines`.

### **The problem with Physical Servers**

In the old days if you wanted to host different applications for your company you would need different physical servers to host each application, and each machine would need a bunch of resources like this:

- **Money:** It's very expansive and not escalable to buy a machine for each application that we need to run;
- **Energy**; 
- **Maintenance**;
- **Network**: Each machine would need to be connected to the network for the application to be able to connect;
- **Idle power**: It was very common that a physical server used just a little percentage of it's processing power, so if one day the number of requests were much bigger then the usual the server wouldn't crash, by doing that the physical servers had a lot of **idle power**.

### **The problem with Virtual machines**

With the creation of `hypervisor`, a technology that works on top of the O.S allowing the `virtualization`  of the physical resources of the system, that is, the creation of the `Virtual Machines` a lot of the problems with the *physical servers* were erased.

#### **Advantages** 

- **Saved resources:** One machine can have a lot of virtual machines;
- **Idle power:** The idle power of each machine is way small if it hosts more than one virtual machines, since they shared the same hardware, leaving less idle power.
- **Creating new aplications:** With V.Ms is way easiar to create new applications, since there's no need to buy another physical server to host it, we just need to create a new V.M. 

#### **Desadvantages**

- **Operatung systems:** Each V.M has it's own O.S and each O.S has it's minimal costs to run, like RAM memory, CPU processing power and memory disc.

- **Maintenance:** Each V.M is a machine and by that we know that it needs to be update regularly, and updating each one of them takes a lot of time and resources. 
    

## Docker?

To understand what docker is we first need to know what `containers` are:

### Container:

Docker Container is a standardized unit which can be created on the fly to deploy a particular application or environment, it's like a virtual machine but without the Operatyng System.

#### Advantages-container

- Containers don't have O.Sm, it uses the O.S of the physical machine that hosts it, which means that we save a lot of resources like RAM, CPU and Memory disc.

- Containers are a lighter-weight, more agile way of handling virtualization.

- Because of the lack of O.S the containers are way faster and easier to build and kill.

#### Why use containers instead of the computer by itself?

Theres a few questions that shows why to use docker containers:

1. What if one application starts to consume too much resources, like CPU? 

    **Answer:** We can delimit the percentage of CPU power that each container can maximaly use

2. What if each application needs a different version of a language?

    **Answer:** We can specify the language version to each container.

3. What if an application freezes your system entirely?

    **Answer:** This can only happen if we don't use docker containers, because with docker containers we can specify the amount of resources that each container can use.

### What is docker?

Docker is a set of technologies that provide modern tools to deploy and run applications. One of the technologies in Docker is the `Docker engine`,
which is what allows us to create the [containers](). the docker engine
is what intermediates the machine-container relationship.


### Docker images:

Docker images are algorithms that says what the docker engine should do to create a new `container`.