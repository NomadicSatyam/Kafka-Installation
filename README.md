# kafka-installation

# Command uses

### Move into Kafka container

```
docker exec -it <kafka_conatiner_id-or-name > /bin/bash

```

### Create Kafka topic here quickstart is topic name

```
kafka-topics --create --topic quickstart --bootstrap-server localhost:9092 --partitions 1 --replication-factor 1

```

### Open New Terminal in Container

```
docker exec -it <kafka_conatiner_id-or-name > /bin/bash

```

### Start Producer app (CLI)

`kafka-console-producer --broker-list localhost:9092 --topic quickstart`

### Open New Terminal in Container

```
docker exec -it <kafka_conatiner_id-or-name > /bin/bash

```
### Start consumer app (CLI)

```
kafka-console-consumer --bootstrap-server localhost:9092 --topic quickstart --from-beginning
```

### List Out All Topics 
```
kafka-topics --list --bootstrap-server <your_bootstrap_server-like-kafkahostname>
```

### Example
```
kafka-topics --list --bootstrap-server broker:9092

```
