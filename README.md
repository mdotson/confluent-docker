Use a docker-machine named dev

```
export DOCKERHOST=`docker-machine ip dev` && docker-compose up

kafka-console-consumer --zookeeper `docker-machine ip dev`:2181 --topic helloworld

kafka-console-producer --broker-list `docker-machine ip dev`:9092 --topic helloworld
```
