# Project Title
Docker is used to containerized application
=>
Docker installation
---------------------------
$ curl -fsSL https://get.docker.com -o get-docker.sh
$ sudo sh get-docker.sh
$sudo usermod -aG docker <your-user>

https://severalnines.com/database-blog/mysql-docker-containers-understanding-basics

=>
Frontend
----------------
FROM centos:7
MAINTAINER "krishnamaram4@gmail.com"
LABEL Purpose=”This is a dockerfile for centos7 and apache httpd server”
RUN yum -y update && yum -y install httpd && yum clean all 
COPY dist /var/www/html
EXPOSE 80
ENTRYPOINT [“ping”]
CMD [“google.com”]


FROM centos
RUN yum install httpd -y
COPY index.html /var/www/html/

CMD [“/usr/sbin/httpd”,” -D”,” FOREGROUND”]
EXPOSE 80

https://linuxtechlab.com/learn-create-dockerfile-example/
https://medium.com/@vi1996ash/steps-to-build-apache-web-server-docker-image-1a2f21504a8e
https://medium.com/@nagarwal/lifecycle-of-docker-container-d2da9f85959
