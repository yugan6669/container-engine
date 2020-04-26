Project Title
==========================

Docker is used to containerized application

Installation and set up
=============================

Step 1:
$yum update -y && yum upgrade -y

$yum install git -y && yum install wget -y && yum install unzip -y && yum install curl -y

Option 1:
$ curl -fsSL https://get.docker.com -o get-docker.sh

$ sudo sh get-docker.sh

Option 2:

$sudo yum install docker -y

Step 2:

$sudo usermod -aG docker <your-user>


EXecution Flow
=========================


Apache HTTP server
------------------------
$git clone https://github.com/krishnamaram2/Container_Engine.git

$cd Container_Engine/src/webserver

$docker image build -t <image_name> .

$docker container run -d --name <container_name> -p 80:80 <image_name>


Apache Tomcat server
-------------------------

docker container run -dit --name t1 -p 8080:8080 krishnamaram2/tomcat:1


MySQL DB server
---------------------

$git clone https://github.com/krishnamaram2/Container_Engine.git

$cd Container_Engine/src/dbserver

$docker image build -t <image_name> .

$docker run --name <container_name> -e MYSQL_ROOT_PASSWORD=Root_123 -d <image_name>

Step 3: create database and user for MySQL

$mysql -u root -p

mysql>create database indigo;

mysql>CREATE USER '<user_name>'@'%' IDENTIFIED BY '';

mysql>GRANT ALL ON . TO ''@'%';

mysql>FLUSH PRIVILEGES;

$git clone https://github.com/krishnamaram2/WebApp.git

$cd WebApp/binary $mysql -u <user_name> -p indigo < indigo.sql







