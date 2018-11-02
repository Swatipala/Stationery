# Stationery-Management
This application is use for Stationery Request Process

Overview
The Stationery service is implemented as a microservice that could be deployed/invoked independent of any client application. Spring and Spring Boot are used to implement the service, Spring Boot provides very nice features regarding packaging and deployment, it packages the whole service as a runnable jar file with the support of its embedded tomcat server. JAX-RS is used to expose the service endpoints as REST. MongoDB is used to persist log messages, Log4j is used as the backbone logging framework.

Technologies
Technology	Purpose
Spring Boot	Simplify the development, packaging and deployment of spring applications by providing fast and ready environment for development, Packages the complete solution as a runnable jar with an embedded tomcat server. http://projects.spring.io/spring-boot/
JAX-RS	Default Java specification for implementing Restful services, I have used the default implementation which is jersey framework. https://jersey.java.net/
MongoDB	A NOSQL scalable DB based on document data model which provides handy scalable data model that fits the need to adapt or change the model later as the requirements evolve, this perfectly fits the need to add more and more data to the logged messages. https://mongolab.com
Mongo Full text search	Deep search in the log messages: http://	docs.mongodb.org/manual/core/index-text/ Provides text indexes to support text search in the whole logged messages.
Spring Data	Provides handy features for data mapping and manipulation backed by MongoDB. http://projects.spring.io/spring-	data-mongodb/
Log4j	The backbone logging framework for the service, both internal logs and application/customer log messages are logged using it.
