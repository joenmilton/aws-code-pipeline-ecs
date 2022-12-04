FROM openjdk:8
EXPOSE 8080
ADD target/first-ecr-ecs-app-0.0.1-SNAPSHOT.jar app.jar 
ENTRYPOINT ["java","-jar","/app.jar"]