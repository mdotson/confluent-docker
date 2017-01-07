Use docker-machine.

docker-compose up

kafka-console-consumer --zookeeper `docker-machine ip dev`:2181 --topic helloworld

kafka-console-producer --broker-list `docker-machine ip dev`:9092 --topic helloworld
