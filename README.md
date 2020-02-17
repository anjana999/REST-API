# REST-API
This repository contains the source code for a maven springboot application to demonstrate GET, PUT, DELETE, POST.

Add java jdk folder of version 13.0.2 and apache maven 3.6.3 in your working directory for running the project.

First create a database in mongodb named Rest and add three records to the collection created, then https://start.spring.io/ create a spring boot application give the package name application name and dependencies required, here we need mongodb and web spring boot, now generate the application and a zip file of the application will be downloaded.

Extract the zip file and open in the visual studio code ide.


Download apache-maven 3.6.3 and jdk-13.0.2 in your working directory to run the application without bugs

In this source code Mongodb connection details and GET, PUT, DELETE, POST methods are all added

To run this application open mvwn.cmd file present in your application with terminal and type cmd in the terminal

Check whether the working directory and and the cmd path are the same. Enter the command mvn spring-boot:run your application will start in your specified port of visual studio code eg. 8080 Enter commands like POST ‘http://localhost:8080/bosses’ PUT ‘http://localhost:8080/bosses/5aecef5b6d55754834124df3' GET ‘http://localhost:8080/bosses/5aecef5b6d55754834124df3’ DELETE ‘http://localhost:8080/bosses/5aecef5b6d55754834124df3’ GET ‘http://localhost:8080/bosses’

To dockerize the project enter the command

mvn clean package

A jar file will be created then enter this command

java -jar ./target/Rest-docker-0.0.1-SNAPSHOT.jar

now create a Dockerfile to build and run the image of the built application

and docker-compose.yml file to specify the version and other requirements

Now you can build and run your application using docker
