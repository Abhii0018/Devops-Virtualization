                                        
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




	




