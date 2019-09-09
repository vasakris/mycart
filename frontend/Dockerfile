#This is dockefile for mycart frontend
FROM centos:7
MAINTAINER vasakris
RUN yum -y update
RUN yum -y install httpd php php-gd php-mysql
ADD code /var/www/html
EXPOSE 80
ENV BACKENDLB=test
ADD scripts /usr/bin
RUN chmod 755 /usr/bin/startapache
CMD ["startapache"]
