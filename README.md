Compile package.

mvn -Dmaven.test.failure.ignore -Dmaven.test.skip=true clean package

Deployment steps:

Copy jars from directories spring-boot-microservice-eureka-naming-server/target, spring-boot-microservice-forex-service/target and spring-boot-microservice-currency-conversion-service/target to server where you want to launch application.

1) Start eaureka server:

java -jar spring-boot-microservice-eureka-naming-server-0.0.1-SNAPSHOT.jar

2) Start forex instance (You can start multiple forex instances)

java -jar spring-boot-microservice-forex-service-0.0.1-SNAPSHOT.jar

3) Start currency converter instance

java -jar spring-boot-microservice-currency-conversion-0.0.1-SNAPSHOT.jar
