FROM openjdk:8u212-jre-alpine

LABEL maintainer="amkcmd@gmail.com"

ADD ./target/account-service.jar /app/

ENV JAVA_OPTS="-server -Xms512m -Xmx512m"

VOLUME /tmp 

EXPOSE 6000

ENTRYPOINT ["sh", "-c", "java ${JAVA_OPTS} -Djava.security.egd=file:/dev/./urandom -jar /app/account-service.jar"]
