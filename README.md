# Microservice using Kafka and Spring Boot

## Description

This is a simple example of a microservice using Kafka and Spring Boot built for the purpose of learning.

## Steps

Add @EnableKafka in the main class to enable Kafka support in your application.

Add @SpringBootApplication in the main class to enable Spring Boot support in your application.

Create a service package in the project root with the name `service`.

Create a service class in the service package with the name `SaveOrderService`.
Add method to store order in the database.

Edit /resources/application.properties and add the following properties:

```properties
spring.kafka.consumer.bootstrap-servers=127.0.0.1:9092
spring.kafka.consumer.auto-offset-reset=earliest
spring.kafka.consumer.key-deserializer=org.apache.kafka.common.serialization.StringDeserializer
spring.kafka.consumer.value-deserializer=org.apache.kafka.common.serialization.StringDeserializer
```

