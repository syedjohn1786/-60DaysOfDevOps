1. What is DevOps ?
DevOps is a process that improves the  organization's delivery of applications by collaborating with various teams such as development team and operations team.

DevOps is not only about improving the ability of delivery applications, it is also about ensuring proper Automation, security, quality, monitoring of the applications.

2. Tools and technologies used in DevOps
Operating System    -   Linux
Version Control     -   Git
CICD                -   Jenkins
Static Code Analysis -  SonarQube
Containerization     -  Docker
Container Orchestration - Kubernetes
IaC                   -  Terraform
Cloud                 -  AWS

3. Networking for DevOps

Here we are going to discuss Networking concepts that are required for a DevOps Engineer

IP Address : A unique code that will be present for each device connected to an Internet

Consider a home having 4 members and those 4 members are using a common Wi-Fi
Suppose we need to block access youtube on the children mobile, how would you do that ?
Therefore we need a unique IP address to do this task.
Its not only about blocking access, it about tracking the activity of the devices.


IPv4 is the standard that is followed to generate unique IP addresses.
It will be in the form of => 172.10.2.4
Maximum number in an IP address will be 255 only ( because 1 byte = 8 bits......1111 1111 (here all the 8 bits we set to 1 , if we calculate this will result in 255))
If the Ip address is 172.600.3.4 => It is invalid IP address ( becaus eof 600)

Subnet : Subnet is basically a small part of the whole network where the IP address are divided or distributed
So each subnet has its own IP Address and we can provide security for the subnet
Its basically the logical separation of IP Address

That logical separation of IP Addresses or method of allocating Ip addresses can be done by CIDR
CIDR - Classless Inter Domain Routing

Below are the important port numbers :

SSH (Secure shell) - 22
HTTP - 80
HTTPS - 443
FTP - 21
FTPS - 990
DNS (Domain Name System) - 53
Jenkins - 8080
SonarQube - 9000