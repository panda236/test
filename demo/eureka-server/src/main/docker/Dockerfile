FROM java:8
VOLUME /tmp
ADD eureka-server-0.0.1-SNAPSHOT.jar eureka-server.jar
RUN bash -c 'touch /eureka-server.jar'
ENTRYPOINT  ["java","-Djava.security.egd=file:/dev/./urandom","-jar","-Dspring.profiles.active=test","/eureka-server.jar"]
EXPOSE 7578
