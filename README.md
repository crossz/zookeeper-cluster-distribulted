# zookeeper-cluster-distribulted

Inspired by https://github.com/mesoscloud/zookeeper.

## diff

- add environment variables for zookeeper port: -e CLIENTPORT
- [ ] port forwarding to replace --net=host

## howto run

```
docker run -d \
-e MYID=1 \
-e SERVERS=node-1,node-2,node-3 \
-e CLIENTPORT=2181 \
--name=zookeeper --net=host --restart=always \
crossz/zookeeper-cluster-distribulted:latest
```
