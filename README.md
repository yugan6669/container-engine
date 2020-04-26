Project Title
==========================

Docker is used to containerized application

Installation and set up
=============================

Step 1:

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

docker container run -dit --name m1 -p 3306:3306 krishnamaram2/mysql:1







