# kafka-setup-demp

- Clone this repository

~ Move inside the cloned directory and execute the following command (Make sure docker is running in your system)
```
docker compose up -d
```
then to access kafka terminal use this command

```
docker exec -it -w /opt/kafka/bin broker sh
```
~ To Add a topic in Kafka,
```
/kafka-topics.sh --create —-topic sample-topic --bootstrap-server broker:29092
```

~ To start consumer on a topic,
```
+/kafka-console-consumer.sh --topic sample-topic --from-beginning --bootstrap-server broker:29092
```
 - To produce a topic
 - ```
   ./kafka-console-producer.sh --topic sample-topic --bootstrap-server broker:29092
   ```
