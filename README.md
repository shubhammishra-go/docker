# Docker

Docker is a set of `platform as a service (PaaS)` products that use `OS-level virtualization`to deliver software in packages called `containers`.The service has both free and premium tiers. The software that hosts the containers is called `Docker Engine`. It was first released in `2013` and is developed by `Docker, Inc`.

Docker is a tool that is used to automate the deployment of applications in lightweight containers so that applications can work efficiently in different environments in isolation. 

![alt text](Docker-Logo.png)



# About PaaS

`Platform as a service (PaaS)` is a category of `cloud computing services` that allows customers to provision, instantiate, run, and manage a modular bundle comprising a computing platform and one or more applications, without the complexity of building and maintaining the infrastructure typically associated with developing and launching the application(s), and to allow developers to create, develop, and package such software bundles.

![alt text](What-Is-PaaS.webp)




# About OS-level virtualization

server virtualization is a technique where the kernel of an operating system allows for multiple isolated user-space instances. These instances run on top of an existing host operating system and provide a set of libraries that applications interact with, giving them the illusion that they are running on a machine dedicated to its use. The instances are known as `Containers`, `Virtual Private Servers` or `Virtual Environments`. 

![alt text](image[30].png)


Operating system level virtualization is achieved by the host system running a single OS kernel and through its control of guest operating system functionality. Under this shared kernel virtualization the virtual guest systems each have their own root file system but share the kernel of the host operating system.


This is a special case of Hosted Virtualization where the hypervisor (the container) has very limited functionality, relying on the Host OS for CPU scheduling and memory management. If you prefer, this method, which uses virtualization at the OS level, doesn’t even include the use of a real hypervisor; instead, the virtualization capabilities are part of the hosting operating system, which performs all the functions of the hypervisor. 

![alt text](image[27].png)

In other words, OS level virtualization is based on the creation of isolated containers or partitions on a single physical server, and the use of OS instances for each guest application environment to work independently of the other partitions. With this technique, you install the virtualization software layer on top of the operating system and all of the guest systems run on top of this layer using the same operating system as the host OS but with each guest having its own resources and running in complete isolation from the other guests.

`NOTE` It can be argued that this is not virtualization in the strict sense of the term; rather a technique that just allows for machine consolidation.


Examples of OS level virtualization are Docker, OpenVZ, Virtuozzo, or Solaris Zones.


Docker can use different interfaces to access virtualization features of the Linux kernel.

![alt text](1920px-Docker-linux-interfaces.svg.png)


#  Advantages of OS Level Virtualization

1. This form of virtualization usually imposes little or no overhead thereby ensuring most of the machine’s resources are available to the applications running in the containers


2. This is a cost-effective and efficient solution for creating similar guests, but it’s only practical for certain situations. It is an ideal approach for web hosting companies which have multiple virtual web servers running on a single box or blade. This is very convenient because patches or modifications can be made to the host server and they will instantly be applied to all of the containers. Another example would be a company that has to manage multiple SQL databases or any other scenario where many similar or identical servers need to be hosted or managed within the same datacenter.


#  Limitations of OS Level Virtualization 

This approach typically limits operating system choice. Containerization usually means that every guest OS must be identical or similar to the host in terms of version number and patch level. For example, with Linux as the host operating system, only Linux distributions can be run as the guest operating systems. This can cause problems if you want to run different applications in the containers, since applications are often certified for only a certain OS version and patch level. It is not possible for a Linux guest system designed for the 3.0.9 version of the kernel to share a 3.1.1 version kernel. 



# How Docker Works ?

Docker works by providing a standard way to run your code. Docker is an operating system for containers. Similar to how a virtual machine virtualizes (removes the need to directly manage) server hardware, containers virtualize the operating system of a server. Docker is installed on each server and provides simple commands you can use to build, start, or stop containers.

![alt text](image.png)


AWS services such as `AWS Fargate`, `Amazon ECS`, `Amazon EKS`, and `AWS Batch` make it easy to run and manage Docker containers at scale.


# Why to use Docker ?

Using Docker lets you ship code faster, standardize application operations, seamlessly move code, and save money by improving resource utilization. With Docker, you get a single object that can reliably run anywhere. Docker's simple and straightforward syntax gives you full control. Wide adoption means there's a robust ecosystem of tools and off-the-shelf applications that are ready to use with Docker.

![alt text](image-1.png)



# When to use Docker ?

You can use Docker containers as a core building block creating modern applications and platforms. Docker makes it easy to build and run `distributed microservices architecures`, `deploy your code with standardized continuous integration and delivery pipelines`, `build highly-scalable data processing systems`, and `create fully-managed platforms for your developers`. The recent collaboration between AWS and Docker makes it easier for you to deploy Docker Compose artifacts to `Amazon ECS` and `AWS Fargate`. 

![alt text](image-2.png)














