FROM openjdk:17-jdk-slim
WORKDIR /app
COPY target/Product_Service-*.jar app.jar
EXPOSE 1234
ENTRYPOINT ["java", "-jar", "app.jar"]