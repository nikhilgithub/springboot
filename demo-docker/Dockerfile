# Start with a base image containing Java runtime
FROM openjdk:8-jdk-alpine

# Add Maintainer Info
LABEL maintainer="marchioni.francesco@gmail.com"

# Add a volume pointing to /tmp
VOLUME /tmp

# Make port 8080 available to the world outside this container
EXPOSE 8080

# The application's jar file
#ARG JAR_FILE=target/demo-docker-0.0.1-SNAPSHOT.jar

# Add the application's jar to the container
#ADD ${JAR_FILE} demo-docker-0.0.1-SNAPSHOT.jar

ENV JAVA_OPTS="-Xms1G -Xmx2G"

# Run the jar fil
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/demo-docker-0.0.1-SNAPSHOT.jar"]
