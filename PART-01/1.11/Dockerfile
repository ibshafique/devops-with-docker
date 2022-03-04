FROM openjdk:8
#exposing port 8080 for the web application
EXPOSE 8080
#setting a working directory for the files to be copied
WORKDIR /usr/src/app 
#copying all the files needed to build the application
COPY ./PART-01/1.11/spring-example-project  .
#building the application
RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]