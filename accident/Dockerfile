FROM eclipse-temurin:17-jdk-jammy
COPY target/*.jar app.jar
EXPOSE 8080
ENV spring.profiles.active=docker
ENTRYPOINT ["java", "-jar", "/app/app.jar"]
