# Memo Kafka Docker
## List all topics:
```
docker exec -it kafka_kafka_1 /bin/bash -c "\$KAFKA_HOME/bin/kafka-topics.sh --list --zookeeper zookeeper:2181"
```

## Consume a message in console mode from the beginning:
```
docker exec -it kafka_kafka_1 /bin/bash -c "\$KAFKA_HOME/bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic nuxeo-batchid1-blobs-r2 --from-beginning"
```

## Description of topics:
```
docker exec -it kafka_kafka_1 /bin/bash -c "\$KAFKA_HOME/bin/kafka-topics.sh --describe --zookeeper zookeeper:2181 --topic nuxeo-batchid1-blobs-r2"
```
