
Unable to delete docker image after running command docker rmi imagename ?
what is the problem and what is solution?

1.Image is running in Container

Solution: 

Stop the running container that are using the image:

#docker ps -a -q --filter ancestor=imagename | xargs docker stop

Then remove these stopped containers:
#docker ps -a -q --filter ancestor=imagename | xargs docker rm 

Remove the image again:

docker rmi imagename

2. Image in Use by stopped container

Solution:

List all containers
#docker ps -a


Identify the container and using the image note down the image id 
#docker rm container_id


3. Image with Dependent child images

Solution:

Identify and remove the child images first
#docker images --filder since=imagename

Remove these child images:
#docker rmi child_image_id

Then remove the parent image:

docker rmi parent_image_name

4. Force remove the image

#docker rmi -f imagename

5. Docker Daemon Issues

Restart the Docker daemon service
#sudo systemctl restart docker

Then remove the image 
#docker rmi imagename