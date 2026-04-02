Importants Commands

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

docker run —name my-container httpd echo “Hello World!” | —name option for give u to given                             name to conatienr 

docker run -e MY_VAR=value httpd env. | the env is execute to display the list of environment                                                   variable in the conatiner, here MY_VAR is value name it can be anything

docker run -it -e MY_NAME=Abhishek ubuntu bash. it will open the container and you can check                                                                           the env variable inside it

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