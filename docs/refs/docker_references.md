## Docker Refs:
http://stackoverflow.com/questions/39229589/how-to-run-application-from-docker-container-from-host-os

## Docker Commands:
* docker build -f <dockerfile> .
* docker build -t <image_name> -f <dockerfile> .
* docker ps -a  # list all containers
* docker stop $(docker ps -a -q) # stop all containers
* docker rm $(docker ps -a -q) # remove all containers
* docker rm <container id>  # remove single container
* docker images # list images
* docker mi <image>   # remove image
