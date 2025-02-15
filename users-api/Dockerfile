FROM openjdk:11

LABEL maintainer="sjbs0212@gmail.com"

VOLUME /tmp

EXPOSE 8083

ARG JAR_FILE=target/users-api-0.0.1-SNAPSHOT.jar

ADD ${JAR_FILE} app.jar

CMD ["java","-jar","/app.jar","JWT_SECRET=PRFT","SERVER_PORT=8083"]
