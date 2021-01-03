FROM java:8-jre

LABEL maintainer="amkcmd@gmail.com"

ADD ./target/auth-service.jar /app/

ENV JAVA_OPTS="-server -Xms512m -Xmx512m"

VOLUME /tmp 

EXPOSE 5000

ENTRYPOINT ["sh", "-c", "java ${JAVA_OPTS} -Djava.security.egd=file:/dev/./urandom -jar /app/auth-service.jar"]
