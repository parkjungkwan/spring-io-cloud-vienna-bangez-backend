FROM openjdk:17-jdk-slim
VOLUME /tmp
RUN apt-get update && apt-get install -y curl
ADD ./build/libs/*.jar tx-service.jar
ENTRYPOINT ["java", "-jar", "/tx-service.jar"]