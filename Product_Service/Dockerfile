# Sử dụng OpenJDK 17 làm base image
FROM openjdk:17-jdk-alpine

# Tạo thư mục làm việc trong container
WORKDIR /app

# Copy file JAR từ thư mục target vào container
ARG JAR_FILE=target/Product_Service-0.0.1-SNAPSHOT.jar
COPY ${JAR_FILE} app.jar

# Mở port trùng với cấu hình Spring Boot
EXPOSE 1234

# Câu lệnh chạy app
ENTRYPOINT ["java", "-jar", "app.jar"]
