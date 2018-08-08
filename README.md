demo-restWS-spring-jersey-jpa2-hibernate
========================================

This demo was forked from this repository: [https://github.com/amacoder/demo-restWS-spring-jersey-jpa2-hibernate](https://github.com/amacoder/demo-restWS-spring-jersey-jpa2-hibernate)

# How to run in OpenShift

## Create a project 
```
oc new-project s2idemo
```

## Using the web console, access your new project and click "Add to Project". Select Mysql (Ephemeral). Use the following parameters:
- Database Service Name = rest_demo
- MySQL Connection Username = rest_demo
- MySQL Connection Password = rest_demo
- MySQL root user Password = rest_demo

## Using the web console, click on Add to Project. Select Wildfly. Use the following parameters:
- Application Name = restdemo
- Git Repository = https://github.com/corpbob/demo-restWS-spring-jersey-jpa2-hibernate.git


Prerequisites:
--
- MySQL 5.5 or 5.6 
- Eclipse
- JDK 1.7 (if you want to use Jetty 9 with the jetty-maven-plugin from project)

Install
--
Create db schema by executing https://github.com/amacoder/demo-restWS-spring-jersey-jpa2-hibernate/blob/master/src/main/resources/input_data/DumpRESTdemoDB.sql against the MySQL database

Run the example
--
- Download/clone the project 
- Import in Eclipse 
- Run Configuration -> Goals "clean install jetty:run"

Go to blog post
--
Visit 
http://www.codingpedia.org/ama/java-persistence-example-with-spring-jpa2-and-hibernate/
for the explanation of the code
