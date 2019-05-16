#My Base Image
FROM ubuntu:latest

#Owner
MAINTAINER Sufia Almas <sufiaalmas4@gmail.com>

#update the apt rpo
RUN apt-get update

#install apache packages
RUN apt-get install apache2 -y

#create a new index page
RUN echo "Welcome to the world of docker " > /var/www/html/index.html

#injecting the application code inside image
COPY sufia.html /var/www/html/info.html

#BRING the apache service
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
