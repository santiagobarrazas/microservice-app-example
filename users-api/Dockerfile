FROM openjdk:8-jdk-alpine

LABEL maintainer="sjbs0212@gmail.com"

VOLUME /tmp

EXPOSE 8083

ARG JAR_FILE=target/users-api-0.0.1-SNAPSHOT.jar

ADD ${JAR_FILE} app.jar

ENV JWT_SECRET=PRFT
ENV SERVER_PORT=8083 

CMD ["java","-jar","/app.jar"]
