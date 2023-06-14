# assignment_demo_2023

![Tests](https://github.com/TikTokTechImmersion/assignment_demo_2023/actions/workflows/test.yml/badge.svg)

This is a demo and template for backend assignment of 2023 TikTok Tech Immersion.

## Installation

Requirement:

- golang 1.18+
- docker
- VSCode (IDE i used for golang)

To install dependency tools:

```bash
make pre
```

## Run

```bash
docker-compose up -d
```

Check if it's running:

```bash
curl localhost:8080/ping
```

## Tasks
Most of the server codes are implemented by the demo template. There are only a few tasks left:
- Setup and configure a datastore (Redis) 
  1) Edit docker-compose.yml to add a Redis server
  2) Setup Redis client in the rpc-server
- Implement handlers in rpc-server
  areYouLucky() is a placeholder function. We need to replace it with our business logic here, i.e writing and reading messages from Redis
  1) Send
  2) Pull

## Updated the following files
1) go.mod
2) go.sum
3) handler_test.go
4) main.go
5) models.go
6) redis.go
7) docker-compose.yml

## Used postman for the API
