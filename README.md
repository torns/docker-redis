# TagoWill/Redis:5.0.0



`Dockerfile` to create a light weight [Docker](https://www.docker.com/) container image for [Redis](http://redis.io/) using Alpine Linux.

**Redis** is an open source, BSD licensed, advanced key-value cache and store. It is often referred to as a data structure server since keys can contain strings, hashes, lists, sets, sorted sets, bitmaps and hyperloglogs. [[Source](https://en.wikipedia.org/wiki/Redis)]

**Alpine Linux** is a [Linux distribution](https://en.wikipedia.org/wiki/Linux_distribution) based on [musl](https://en.wikipedia.org/wiki/Musl) and [BusyBox](https://en.wikipedia.org/wiki/BusyBox), primarily designed for "[power users](https://en.wikipedia.org/wiki/Power_user) who appreciate security, simplicity and resource efficiency". [[Source](https://en.wikipedia.org/wiki/Alpine_Linux)]



The idea is to create from scratch a light weight container using local images. It's useful when need to create a docker container image in a machine that doesn't have internet connections or it's not allowed to connect to DockerHub (Enterprise/Companies purposes).

Also, having the most updated version of Redis.

Current versions used:

|     Alpine Linux     | Redis |
| :------------------: | :---: |
| library-3.8 (x86_64) | 5.0.0 |



This project is still in development. So, bear with me with the missing docs, it will be available soon.

Please feel free to help or give ideas to this by opening issues and pull-requests.



# Getting started

Steps needed to build an image and/or run a container.



## Build an container image

Before running any container or docker-compose we need to build an image

```bash
docker build -t tagowill/redis:latest -t tagowill/redis:11.0 .
```



## Run container

To run container just with PostgreSQL use the docker-compose:

```bash
docker-compose up -d
```

or

```bash
docker run --rm --name <containerName> tagowill/redis:latest
```

