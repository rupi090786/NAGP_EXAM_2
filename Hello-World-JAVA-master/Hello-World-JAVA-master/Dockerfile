FROM openjdk:8-jdk-alpine
MAINTAINER Rupesh Kumar
WORKDIR /rupeshkumar01
RUN addgroup -S spring && adduser -S spring -G spring
USER spring:spring
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","app.jar"]