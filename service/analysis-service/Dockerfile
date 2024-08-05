FROM openjdk:17-jdk-slim
VOLUME /tmp
RUN apt-get update && apt-get install -y curl
ADD ./build/libs/*.jar analysis-server.jar
ENTRYPOINT ["java", "-jar", "/analysis-server.jar"]