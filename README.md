# Realtime push notification with Redis

This is a simple dockerized push notification service using redis pub/sub.


### Installation

It requires docker, docker compose to run.

Spin up the compose  - 

```sh
$ docker-compose up -d 
```

### Usage

 - Go to localhost:3000
 - Open interactive shell of `notfredis` container, then open redis-cli
```sh
$ redis-cli
```
 - Using the `redis-cli`, publish a message to notifications channel 
```sh
$ PUBLISH app:notifications  "hiii"
```
 - Done ! See your notifications in real time.

![](demo.gif)
