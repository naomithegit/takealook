### Use an official OpenJDK runtime as a parent image
##FROM openjdk:11-jre-slim
##
### Set the working directory in the container
##WORKDIR /app
##
### Copy the jar file into the container at /app
###COPY target/client-application-0.0.1-SNAPSHOT.jar /app/client-application.jar
##COPY target/client-application-0.0.1-SNAPSHOT.jar /app/client-application.jar
##
##
### Run the jar file
##CMD ["java", "-jar", "client-application.jar"]
#
## Use an official OpenJDK runtime as a parent image
#FROM openjdk:11-jre-slim
#
## Set the working directory in the container
#WORKDIR /app
#
## Copy the packaged jar file into the container
#COPY target/client-application-0.0.1-SNAPSHOT.jar /app/client-application.jar
#
## Make port 8080 available to the world outside this container
#EXPOSE 8080
#
## Run the jar file
#ENTRYPOINT ["java", "-jar", "/app/client-application.jar"]


FROM openjdk:11-jre-slim

# Set the working directory in the container
WORKDIR /app

# Copy the packaged jar file into the container
COPY target/client-application-0.0.1-SNAPSHOT.jar /app/client-application.jar

# Make port 8080 available to the world outside this container
EXPOSE 8080

# Run the jar file
ENTRYPOINT ["java", "-jar", "/app/client-application.jar"]