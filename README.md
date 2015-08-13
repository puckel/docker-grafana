## Grafana Dockerfile


This repository contains **Dockerfile** of [Grafana(2.1.0)](http://grafana.org/) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/puckel/docker-grafana/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).


### Base Docker Image

* [puckel/docker-base](https://registry.hub.docker.com/u/puckel/docker-base/)


### Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/puckel/docker-grafana/) from public [Docker Hub Registry](https://registry.hub.docker.com/):
 `docker pull puckel/docker-grafana`

Alternatively, you can build an image from [Dockerfile](https://github.com/puckel/docker-grafana)

### Usage

```bash
    docker run -d \
        --name grafana \
        -p 3000:3000 \
        --link graphite:graphite \
        puckel/docker-grafana
```
