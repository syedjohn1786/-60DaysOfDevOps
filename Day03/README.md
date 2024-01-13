Kubernetes
======================

The pre-requisite for learning kubernetes is Docker.

Docker is basically a container platform where as Kubernetes is container orchestration platform.

Containers are Ephemeral in nature ( i.e short life) , which means containers die and revive anytime.

Problems with Docker Containers :
=====================================

1. Single Host Nature of Docker Containers

Consider a Host machine on which you installed a Docker and created 100 containers on that Docker. Assume the 1st container is consuming a very big amount of memory and this may impact 99th container and the 99th container will not get started and die. Due to memory issue or the image is not getting pulled , the container will immediately die. This is due to Single Host nature of Docker containers.

2. Auto Healing

Consider a user have killed a container in which the application is running. So now , we cant access the application because the container is killed. The application will be up and running only if any DevOps engineer manually start the container which is killed. If this process is done without manual intervention, then it is called as Auto Healing.

Auto Healing is the mechanism of starting the container by itself if it was down.

3. Auto Scaling

Consider a Host machine on which you installed a Docker and created 5 containers. Assume you run an e-commerce application on these 5 containers. During any festive season the usage of the application by the customers will be high and 5 containers may not handle all the customers requests and eventually load increases and it leads to application break. 

One way to solve this issue was manually you increase the no of containers and keeps the application up and Running

The other way is Auto scaling. We cant predict the usage of customers on special occasions and we need to automate this process i.e whenever load gets increased automatically the no of containers must increase and the application must be up and running.

Docker doesnt support the above 2 ways.

4. Docker doesn't supporrt Enterprise level standard ( i.e no support like Load balancing, firewalls, scaling, Auto scaling, API Gateway). This is the main Reason that "Docker is never used in Production".

If you are using simple Docker platform then Docker doesn't support Load balancing, firewalls, scaling, Auto scaling, API Gateway.
 
Note : If you are using Docker Swarm, you can do Load balancing, Auto scaling etc.


These are the Drawbacks of Docker and we need Kubernetes to solve these drawbacks.


