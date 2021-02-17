# Kafka Services 

## List of Commands Used to Start Kafka Services

- Starting the zookeeper service  
```.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties```

- Starting the kafka service  
```.\bin\windows\kafka-server-start.bat .\config\server.properties```

- Creating a unique topic  
```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic big-data-tools ```

- Listing all the available topics  
```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list```

- Starting the producer from unique topic  
 ```.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic big-data-tools```
 
- Starting the consumer from unique topic  
``` .\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic big-data-tools --from-beginning```
