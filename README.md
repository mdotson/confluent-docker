## Docker for mac
`export DOCKERHOST=`ipconfig getifaddr en0` && docker-compose up`

## Docker-machine
`export DOCKERHOST=`docker-machine ip dev` && docker-compose up`

## Linux
`export DOCKERHOST=`hostname --ip-address` && docker-compose up`

# Run it
```
kafka-console-consumer --zookeeper $DOCKERHOST:2181 --topic helloworld

kafka-console-producer --broker-list $DOCKERHOST:9092 --topic helloworld
```
