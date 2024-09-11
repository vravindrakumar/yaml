

   $ host name
   $if config
   $sudo apt install net-tools
   $if config
   $docker network ls
   $sudo su
   $ docker network ls
   $docker network create my-bridge-network
   $docker ps 
   $docker ps -a 
   $docker images
   $docker run -d --name container1 --network my-bridge-network httpd
   $docker ps 
   $docker stop container1
   $docker ps
   $docker start container1
   $docker images
   $docker pulltomcat
   $docker images
   $docker run -d --name tomcat01 -p 8081:8080 tomcat:latest
   $docker run -d --name container3 --network my-bridge-network  -p 8080:80 httpd
   $docker network ls
   $docker ps



