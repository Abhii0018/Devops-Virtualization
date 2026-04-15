                                        
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


