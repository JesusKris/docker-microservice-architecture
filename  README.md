<!-- ctrl + shift + v to preview -->
# play-with-containers


## play-with-containers is a practical task where I was tasked to deploy microservices and a gateway using docker compose as a student project [@kood/Johvi](https://kood.tech/).   

### --> [Audit Video](https://www.youtube.com/watch?v=a6JRrjLpji4) <--

## **Table of Contents**
* ### [Terminology](#terminology-1)
* ### [Contact](#contact-1)
* ### [Usage](#usage-1)


## **Terminology**

- Docker containers are lightweight, portable, and self-sufficient units that package software and all its dependencies, including the runtime, system tools, libraries, and settings, to run reliably and consistently across different environments. 
   <br><br>
- Containers are best suited for modern, lightweight, and scalable applications, while virtual machines are more suitable for legacy applications and workloads requiring stronger isolation.
   <br><br>
- Docker is an open-source platform that automates the deployment, scaling, and management of applications using containerization technology. It allows developers to package their applications and all their dependencies into a single container image, ensuring consistent and reproducible deployments across various environments.
   <br><br>
- Microservices architecture is a software development approach that structures an application as a collection of small, independent, and loosely coupled services. In a microservices architecture, each service represents a specific business capability and runs as a separate process. These services communicate with each other through well-defined APIs, typically over HTTP or message queues.
   <br><br>
- Teams use microservices architecture primarily because it enables them to work more independently and efficiently. With microservices, different teams can focus on developing and maintaining specific services without interfering with each other's work.
   <br><br>
-  Queues enable asynchronous communication between different services or applications. One service can place a message in the queue, and another service can process it at a later time, decoupling their activities and allowing them to work independently.
   <br><br>
-  RabbitMQ is an open-source message broker software that implements the Advanced Message Queuing Protocol (AMQP). It serves as a messaging middleware that enables communication and coordination between different components or services in a distributed system. 
   <br><br>
-  A Dockerfile is a text file that contains a set of instructions used to build a Docker image. 
   <br><br>
-  A Docker volume is a mechanism provided by Docker to persistently store data generated and used by Docker containers. It allows containers to share and manage data independently of the container's lifecycle.
   <br><br>
-  Docker network is a feature that allows containers to communicate with each other and with external networks in a secure and isolated manner. 
   <br><br>
-  A Docker image is a lightweight, standalone, and executable software package that contains everything needed to run an application, including the code, runtime, libraries, dependencies, and system tools.
   <br><br>
-  Using Docker images, developers can package applications and their dependencies together, making it easier to manage and deploy applications in a consistent and scalable manner.
   <br><br>
-  Public Docker images can be found on Docker Hub, which is the official repository for Docker images. Docker Hub is a cloud-based registry that hosts a wide variety of pre-built images, created by both individual developers and organizations. 

## **Usage**

Install VirtualBox
```
sudo apt install virtualbox
```

Install vagrant
```
sudo apt install vagrant
```

Deploy the microservices
```
vagrant up --provider virtualbox
```

## **Contact**
### Made by [nimi25820](https://01.kood.tech/git/nimi25820)