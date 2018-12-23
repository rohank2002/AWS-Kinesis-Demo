# AWS-Kinesis-Demo
Basic configuration and demonstration  of AWS Kinesis 
First create a Kinesis stream using the following ``` aws-cli ``` command
```sh
aws kinesis create-stream --stream-name python-stream --shard-count 1
```
The kinesis_producer.py will put records to the stream continuosly every 5 seconds
The kinesis_consumer.py will start consuming as the producer puts to the stream
