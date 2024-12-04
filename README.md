# bigdata-demo

Apache flume (namenode):

```
curl https://archive.apache.org/dist/flume/1.9.0/apache-flume-1.9.0-bin.tar.gz -o apache-flume-1.9.0-bin.tar.gz

tar xzf apache-flume-1.9.0-bin.tar.gz

export FLUME_HOME=/apache-flume-1.9.0-bin

$FLUME_HOME/bin/flume-ng version

docker cp flume_kafka.conf namenode:/apache-flume-1.9.0-bin/conf/flume_kafka.conf

bin/flume-ng agent --conf conf --conf-file conf/flume_kafka.conf --name agent -Dflume.root.logger=INFO,console
```

Apache kafka:
```
kafka-console-producer --topic my-topic --bootstrap-server localhost:19092


```
