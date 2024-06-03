FROM openjdk:15-jdk-slim
COPY target/*SNAPSHOT.jar /app/app.jar
EXPOSE 8080
ENV TZ=Asia/Seoul
ENTRYPOINT ["java","-Xmx400M","-Djava.security.egd=file:/dev/./urandom","-jar","/app/app.jar"]