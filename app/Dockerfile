FROM maven:3.6.1-jdk-8-alpine AS build
RUN mkdir -p /workspace
WORKDIR /workspace
COPY . /workspace
RUN mvn package spring-boot:repackage

FROM amazoncorretto:8-alpine
COPY target/spring-boot-app-0.0.1-SNAPSHOT.war /app.war
ENV JAVA_HOME /usr/
EXPOSE 8081
CMD java -jar -Dspring.profiles.active=default /app.war