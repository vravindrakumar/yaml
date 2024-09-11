Take ubuntu latest OS from hub.docker.com
FROM ubuntu:latest

#Update the ubuntu os
RUN  apt-get update &&  \
      apt-get install -y openjdk-11-jdk wget  &&  \
      apt-get clean
#Create tomcat directory is /opt
RUN mkdir /opt/tomcat

#Configure working directory tomcat
WORKDIR /opt/tomcat

#Download link for the tomcat
RUN wget https://dlcdn.apache.org/tomcat/tomcat-11/v11.0.0-M22/bin/apache-tomcat-11.0.0-M22.tar.gz


#Un-tar the tar.gz file
RUN tar -zxvf apache-tomcat-11.0.0-M22.tar.gz

#move the tomcat files to /opt directory
RUN mv /opt/tomcat/apache-tomcat-11.0.0-M22/* /opt/tomcat

#set env variable
ENV echo 'export CATALNA_HOME= "/opt/tomcat"'   >> ~/. bashrc
ENV echo  'export PATH="$PATH:$CATALINA_HOME/bin"'  >> ~/.bashrc
ENV source  ~/.bashrc

#Expose tomcat port number
EXPOSE 8080

#Start the tomcat service
CMD ["/opt/tomcat/bin/catalina.sh" , "run"]
