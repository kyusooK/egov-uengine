FROM eclipse-temurin:17-jdk-jammy
COPY target/*.jar app.jar
EXPOSE 8080
ENV spring.profiles.active=docker
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
ENTRYPOINT ["java", "-jar", "/app/app.jar"]