# Docker Java Demo

This project is meant to demonstrate the use of docker-compose and a Dockerfile to build a java application and then start up the container.

## Prerequisites

In order to run this application you need to install two tools: **Docker** & **Docker Compose**.

Instructions how to install **Docker** on [Ubuntu](https://docs.docker.com/install/linux/docker-ce/ubuntu/), [Windows](https://docs.docker.com/docker-for-windows/install/), [Mac](https://docs.docker.com/docker-for-mac/install/).

**Docker Compose** is already included in installation packs for *Windows* and *Mac*, so only Ubuntu users needs to follow [this instructions](https://docs.docker.com/compose/install/).

## Build and Start

This command should build the maven project and deploy it to the container.

``` bash
docker-compose up --build
```

## Start Only

After the app has been built, it can be just started.

``` bash
docker-compose up
```

## Stop

Always stop the last docker compose start command before issuing another.

> make sure to stop every `docker-compose up` command

``` bash
docker-compose down
```

## Test build

If all went well, you should be able to view the data results at this url:

**http://localhost:8081/springbootapp/employees**
