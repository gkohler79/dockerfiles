FROM openjdk:8-jdk-alpine
LABEL maintainer="grant.kohler@gmail.com"
VOLUME /tmp
EXPOSE 8080
ARG JAR_FILE=target/family-budget-1.0.0.jar
ADD ${JAR_FILE} family-budget.jar
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/family-budget.jar"]
