# Docker Java Demo

This project is meant to demonstrate the use of docker-compose and a Dockerfile to build a java application and then start up the container.

## Build and Start

``` bash
docker-compose up --build
```

## Start Only

``` bash
docker-compose up
```

## Stop

> make sure to stop every `docker-compose up` command

``` bash
docker-compose down
```

## Test build

If all went well, you should be able to view the data results at this url:

**http://localhost:8081/springbootapp/employees**
