FROM openjdk:8-jdk-alpine
VOLUME ["/tmp"]
ADD twig-config-0.0.1-SNAPSHOT.jar app.jar
ENTRYPOINT ["java", "-agentlib:jdwp=transport=dt_socket,address=5005,server=y,suspend=n", "-Dspring.profiles.active=prod", "-Djava.security.egd=file:/dev/./urandom", "-jar","/app.jar"]
MAINTAINER Peng Wang "wpcfan@gmail.com"
