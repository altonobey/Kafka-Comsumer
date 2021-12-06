# Kafka-Comsumer

Start Zookeeper:
bin/zookeeper-server-start.sh config/zookeeper.properties

Start Kafka Server:
bin/kafka-server-start.sh config/server.properties

Create Kafka Topic: /n
bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic Kafka_Example

Consume from the Kafka Topic via Console:
bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic Kafka_Example --from-beginning

Check existing topics:
bin/kafka-topics.sh --bootstrap-server localhost:9092 --list

Delete Kafka Topic:
bin/kafka-topics.sh --delete --bootstrap-server localhost:9092 --topic Kafka_Example
