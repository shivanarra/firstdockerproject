FROM centos:latest
MAINTAINER shivadevops9@gmail.com
RUN yum -y update
RUN mkdir /opt/config
ADD config /opt/config
RUN yum -y install `cat /opt/config/packages`
ADD code /var/www/html/
EXPOSE 80
CMD ["apachectl","-D","FOREGROUND"]