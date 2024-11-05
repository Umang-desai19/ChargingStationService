# ChargingStationService
1 **Technologies used:**<br>
Java 21<br>
Spring Boot<br>
KStreams<br>
Microservices<br>

**Kafka Topics**:<br>
**charging-status**: ChargingUpdateService will continuously publish messages to this topic for all the requests.<br>
**charging-status-stream**: ChargingUpdateService will read data from above topic and publishes updated message using KStream to this topic. <br>
                            ChargingProcessorService consumes messages from this topic and updates required details in database.<br>

**Services Will be available on locahost on following ports:**<br>
<br>
Start the services as per port details given below:<br>
<br>
Zookeeper: 2181<br>
Broker-1: 9092<br>
Broker-2: 9093<br>
Kafka-ui: 8081<br>
ChargingStationService: 8056<br>
ChargingUpdateService: 8052<br>
ChargingProcessorService: 8053<br>
<br>
