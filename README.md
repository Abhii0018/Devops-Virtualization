                                        
                                                        Important Commands


docker history httpd. —show the history   

docker pull httpd.     —for pull the docker image

docker images.         —show all the images inside docker

docker run.     —used to create and start docker image

docker run -it.    - it is used for run in iterative way allowing you to interact with container through command line

docker run -p.    maps a host port to a container port

docker run -d. runs in background

docker run —rm automatically remove the container when it exists

docker run —name. specifies a name for the container 

docker run httpd echo “Hello World!”    in this case new conatiner will be create 

docker run —name my-container httpd echo “Hello World!” | —name option for give u to given name to conatienr 

docker run -e MY_VAR=value httpd env. | the env is execute to display the list of environmentvariable in the conatiner, 
                                   here MY_VAR is value name it can be anything

docker run -it -e MY_NAME=Abhishek ubuntu bash |. it will open the container and you can check                                                                                                                   the env variable inside it

docker run -e APP_ENV=production -e APP_VERSION=1.0 nginx

or 

docker run -d\

            -e APP_VERSION=1.0 nginx\

            -e MY_NAME=Abhishek ubuntu bash

docker ps  — show all running conatiner

docker run -it -e COLLEGE=CSE ubuntu /bin/bash

docker ps -a | list all container running/existed/stopped

docker rmi 8fevcehrjk | remove docker image

docker rmi -f <image_id> | remove the image forcefully

docker unpause <container_id/name>. | unpause a paused container

docker kill <container_id/name>.  | kill a container(force stop)

docker rm <container_id/name> | Remove a container

docker container prune. | Remove all stopped containers

                                TASK 1:-
You are a DevOps trainee and need to deploy the Apache HTTP Server (httpd) using Docker for testing a static website. Pull the Apache server image from Docker Hub, create a container named apache-web, and run it in detached mode. Map port 8081 on the host machine to port 80 inside the container so that the website can be accessed through a browser.
Tasks:
Pull the Apache (httpd) Docker image.
Verify that the image is successfully downloaded.
Run the container with the specified name and port mapping.
Check the list of running containers.
Access the Apache web server using a browser.
<img width="445" height="157" alt="Screenshot 2026-04-15 at 5 10 55 PM" src="https://github.com/user-attachments/assets/208bf7aa-a2bd-411c-b1e7-767bf15fca99" />


<img width="1033" height="339" alt="Screenshot 2026-04-15 at 5 02 51 PM" src="https://github.com/user-attachments/assets/6867aa1e-7b20-47f7-8c64-6fc290cf90f0" />

                       Task  2:
                       
Deploy a MySQL database server using Docker. Configure the container with environment variables to set the root password, create a database named college, and create a user with credentials. Run the container in detached mode and verify that the database is running successfully.

<img width="998" height="389" alt="Screenshot 2026-04-15 at 5 18 57 PM" src="https://github.com/user-attachments/assets/4f47c16f-9ac5-439a-9c90-d54ad605d17d" />




<img width="936" height="288" alt="Screenshot 2026-04-15 at 5 20 26 PM" src="https://github.com/user-attachments/assets/233de7c7-51aa-44ea-940b-7eb3dc7c0e7f" />



<img width="886" height="369" alt="Screenshot 2026-04-15 at 5 20 49 PM" src="https://github.com/user-attachments/assets/12330977-4ad2-493b-b75b-58c2e434e99b" />



                                 Task 3:-
  Run an Ubuntu container using Docker, pass an environment variable COLLEGE=CSE, verify it inside the container, and observe what happens after stopping the container.
  
<img width="1004" height="386" alt="Screenshot 2026-04-15 at 5 25 59 PM" src="https://github.com/user-attachments/assets/55b66104-50ea-47b9-84da-0af48cd7ff58" />

After resteart----------


<img width="844" height="98" alt="Screenshot 2026-04-15 at 5 28 16 PM" src="https://github.com/user-attachments/assets/a499ae7b-9474-483f-94f8-9100dc76a1bc" />



                                     Task 4:-
Run a Docker container named DB-app using the MongoDB image and expose it so that it can be accessed from the host system.


<img width="1024" height="392" alt="Screenshot 2026-04-15 at 5 33 06 PM" src="https://github.com/user-attachments/assets/3e455c35-1bc6-49e9-a80a-0849bde46d61" />


                              Task 5:-
You are a DevOps engineer in a startup company. The development team asks you to quickly deploy a simple web page that displays the message:

Use the official httpd Docker image.
Run the container so it is accessible on port 8080 of the host machine.
Create or update an HTML file inside the container to display the required message.
Verify the output using a command-line tool.
Properly stop and remove the container after testing.


<img width="528" height="227" alt="Screenshot 2026-04-15 at 5 36 08 PM" src="https://github.com/user-attachments/assets/158b5153-f42e-43e0-b7ae-a6956317e918" />



<img width="1034" height="383" alt="Screenshot 2026-04-15 at 5 35 35 PM" src="https://github.com/user-attachments/assets/dd5bd2db-84da-4a49-8aeb-fb8f53aeb021" />

                                                        Task 6:-
                                                        
  How would you use the docker run command with -it, -e, -v, and --name to:
•	Set an environment variable APP_ENV=production.	
•	Bind a local directory /app/data to /data inside the container.	
•	Name the container my_app.	


<img width="684" height="230" alt="Screenshot 2026-04-15 at 5 45 35 PM" src="https://github.com/user-attachments/assets/2f4c99a5-327e-490e-8dbb-95f6766ddcf1" />


In another terminal:---


<img width="815" height="184" alt="Screenshot 2026-04-15 at 5 45 48 PM" src="https://github.com/user-attachments/assets/c37e6abe-8232-4b30-8993-3e288141b816" />

Important Container command:---------------

Unpause a paused container 
docker unpause <container_id/name>

Kill a container (force stop) 
docker kill <container_id/name>

Remove a container 
docker rm <container_id/name>

Remove all stopped containers 
docker container prune

                                 Task 7:--
You need to start a new container using the nginx image while setting an environment variable ENV_MODE=production. Write the docker run command to achieve this.


<img width="591" height="186" alt="Screenshot 2026-04-15 at 5 55 10 PM" src="https://github.com/user-attachments/assets/4f36a205-2790-4c56-b9c5-bd70a26617e6" />


                                  Task 8:-------

								  
You are a DevOps engineer at a university. The web development team has built a simple HTML-based portal and wants it deployed using Docker.
Use the official httpd image.
Name the container college_portal.
Run it in detached mode.
Expose container port 80 to host port 8080.
Set environment variable ENV=production.
Attach a Docker volume named portaldata to store website files.
Modify the index.html file inside the container.
Verify the output in the browser.
Check logs if the page is not loading.
Stop and remove the container.
Remove the volume and image after testing.	



<img width="1065" height="394" alt="Screenshot 2026-04-15 at 6 01 10 PM" src="https://github.com/user-attachments/assets/96fb42e3-e15a-4c17-9815-90de90475928" />


<img width="544" height="181" alt="Screenshot 2026-04-15 at 6 01 30 PM" src="https://github.com/user-attachments/assets/6dfc2439-3153-4484-861e-327f82f028cd" />


																		   Unit-3

Monolithic vs Microservices
Introduction
Software architecture has evolved significantly over time:

1980s–1990s → Monolithic applications on physical servers
2000s → N-tier applications with virtualization
Present → Microservices running in containers using Docker and Kubernetes
Microservices architecture became popular because modern applications require scalability, flexibility, and faster deployment.

Monolithic Architecture
A monolithic application is built as a single unified application where all components are tightly coupled.

It mainly contains:

User Interface (UI)
Business Logic
Database Access Layer
All modules are developed and deployed together.

Example of Monolithic Application
An E-commerce application where:

Frontend
Backend
Authentication
Payment
Database
are combined into one large application.

Advantages of Monolithic Architecture
Simple deployment
Easy debugging and testing
Faster internal communication
Suitable for small applications
Disadvantages of Monolithic Architecture
Difficult to scale specific modules
Large codebase becomes hard to manage
Technology upgrades become difficult
One failure can affect entire application
Slower development for large teams
Microservices Architecture
Microservices architecture divides an application into multiple small independent services.

Each service:

Performs a specific business task
Runs independently
Communicates using APIs
Can use its own database
Example of Microservices
An online shopping platform may contain:

User Service
Product Service
Payment Service
Order Service
Recommendation Service
Each service works independently.

Advantages of Microservices
Advantage	Description
Scalability	Services can scale independently
Independent Deployment	Update one service without affecting others
Fault Isolation	Failure in one service does not stop entire system
Technology Flexibility	Different technologies can be used
Faster Development	Teams can work independently
Easier Maintenance	Small services are easier to manage
Disadvantages of Microservices
Complex architecture
Difficult service communication
More deployment management
Monitoring becomes challenging
Requires container orchestration tools
Monolithic vs Microservices
Feature	Monolithic	Microservices
Architecture	Single application	Multiple independent services
Scalability	Entire app scaled together	Individual services scaled
Deployment	Single deployment	Independent deployment
Fault Isolation	Low	High
Flexibility	Less flexible	Highly flexible
Maintenance	Difficult for large apps	Easier due to smaller services
Technology Stack	Usually single stack	Multiple stacks possible
Role of Containers in Microservices
Microservices are commonly deployed using containers such as Docker.

Benefits:

Lightweight deployment
Faster startup time
Isolation between services
Better resource utilization
Easy scalability
Kubernetes is often used to manage multiple containers.

Real-World Examples
Netflix
Amazon
Flipkart
Swiggy
Zomato
These platforms use microservices to handle millions of users efficiently.

Important Viva Questions
1. What is a monolithic application?
A monolithic application is a single unified application where all components are tightly coupled and deployed together.

2. What are microservices?
Microservices are small independent services that work together to form an application.

3. Why are microservices preferred over monolithic architecture?
Because they provide scalability, flexibility, independent deployment, and fault isolation.

4. What is fault isolation in microservices?
Failure of one service does not affect the complete application.

5. Why are containers used in microservices?
Containers provide lightweight, isolated, and portable environments for running services.

Conclusion
Monolithic architecture is simple and suitable for small applications, while microservices architecture is better for large-scale modern applications requiring scalability, flexibility, and faster deployment.

                                              Container

Containers
Introduction
Containers are lightweight virtualization technologies that allow multiple isolated applications to run on a single operating system.

Containers package:

Application code
Dependencies
Libraries
Runtime environment
This makes applications portable and consistent across different systems.

What is a Container?
A container is an isolated environment that shares the host operating system kernel while running applications independently.

Containers are widely used in DevOps and cloud computing because they are:

Lightweight
Fast
Portable
Scalable
Features of Containers
OS-level virtualization
Lightweight compared to Virtual Machines
Fast startup time
Efficient resource utilization
Portable across environments
Isolation between applications
Containers vs Virtual Machines
Feature	Containers	Virtual Machines
Virtualization Type	OS-level virtualization	Hardware-level virtualization
Size	Lightweight	Heavy
Startup Time	Seconds	Minutes
Resource Usage	Low	High
OS Requirement	Shares host kernel	Separate guest OS
Performance	Faster	Slower compared to containers
Working of Containers
Containers use:

Namespaces → for process isolation
Control Groups (cgroups) → for resource limits
Container Runtime → to run containers
The host operating system kernel is shared among all containers.

Advantages of Containers
Faster deployment
Better resource utilization
Easy scalability
Consistent development environment
Simplified application deployment
High portability
Containers and Microservices
Containers are commonly used to deploy microservices.

Each microservice can run inside its own container with:

Required dependencies
Runtime environment
Libraries
Benefits:

Independent deployment
Fault isolation
Better scalability
Faster updates
Docker and Kubernetes
Docker
Docker is a containerization platform used to:

Build containers
Run containers
Manage container images
Kubernetes
Kubernetes is a container orchestration tool used to:

Manage multiple containers
Auto-scale applications
Self-heal failed containers
Handle container networking
Real-World Uses of Containers
Containers are widely used in:

Cloud applications
CI/CD pipelines
Microservices architecture
DevOps automation
Scalable web applications
Companies using containers:

Netflix
Amazon
Google
Spotify
Important Viva Questions
1. What is a container?
A container is a lightweight isolated environment used to run applications along with their dependencies.

2. Why are containers lightweight?
Because they share the host operating system kernel instead of running a separate OS.

3. What is the difference between containers and VMs?
Containers share the host OS kernel while VMs use separate guest operating systems.

4. What is Docker?
Docker is a platform used for containerization.

5. What is Kubernetes?
Kubernetes is a container orchestration platform used to manage multiple containers.

6. Why are containers useful in microservices?
Containers provide portability, scalability, and isolation for microservices deployment.

Conclusion
Containers provide lightweight, fast, and portable application deployment environments. They are a core technology in modern DevOps and microservices architecture.


<img width="697" height="556" alt="Screenshot 2026-05-21 at 12 23 15 PM" src="https://github.com/user-attachments/assets/bba19f63-6ffc-46b8-90c9-358a8c015283" />

# Practical 01 - Docker Compose Basics

# Aim

To understand the basics of Docker Compose and deploy an Nginx container using a docker-compose.yml file.

---

# Problem Statement

Create a Docker Compose configuration file to run an Nginx web server container and verify the deployment using Docker Desktop and browser.

---

# Requirements

- Docker Desktop
- Docker Compose
- VS Code

---

# Docker Compose File

```yaml
services:
  web:
    image: nginx
    ports:
      - "8080:80"
```

---

# Explanation

## services
Defines all containers used in the application.

---

## web
Name of the service.

---

## image: nginx
Pulls official Nginx image from Docker Hub.

---

## ports
Maps host port to container port.

```text
8080 → Host Port
80 → Container Port
```

---

# Steps Performed

## Step 1: Open Project Folder

Navigate to:

```text
C:\Users\Lenovo\OneDrive\Desktop\devops2\unit3\03-Docker-Compose-Basics
```

---

## Step 2: Create docker-compose.yml

Created Docker Compose configuration file.

---

## Step 3: Run Docker Compose

Command used:

```bash
docker compose up -d
```

---

## Step 4: Verify Running Container

Command used:

```bash
docker compose ps
```

---

## Step 5: Open Browser

Visited:

```text
http://localhost:8080
```

Verified Nginx web server output.

---

# Output Screenshots

## 1. Docker Compose File

![Compose File](img2.png)

---

## 2. Docker Compose Up

![Docker Compose Up](img3.png)

---

## 3. Running Containers

![Docker Compose PS](img4.png)

---

## 4. Docker Desktop Running Container

![Docker Desktop](screenshots/img5.png)

---

## 5. Browser Output

![Nginx Output](screenshots/img6.png)

---

# Result

Successfully created and deployed an Nginx container using Docker Compose.

---

# Conclusion

Docker Compose simplifies container deployment and management using a single YAML configuration file.










