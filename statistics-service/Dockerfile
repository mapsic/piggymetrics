FROM java:8-jre
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/statistics-service.jar /app/
CMD ["java", "-Xmx1g", "-jar", "/app/statistics-service.jar"]

EXPOSE 7000
