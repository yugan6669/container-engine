# Project Title
Docker is used to containerized application
=>
Docker installation
---------------------------
$ curl -fsSL https://get.docker.com -o get-docker.sh
$ sudo sh get-docker.sh
$sudo usermod -aG docker <your-user>


Apache HTTP server
------------------------
docker container run -dit --name h1 -p 80:80 krishnamaram2/http:1


Apache Tomcat server
-------------------------
docker container run -dit --name t1 -p 8080:8080 krishnamaram2/tomcat:1

MySQL DB server
---------------------
docker container run -dit --name m1 -p 3306:3306 krishnamaram2/mysql:1
