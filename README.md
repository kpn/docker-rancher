# Docker-Rancher-Helm

## Overview

Docker image containing rancher client, helm client and kubectl. This image is available on [DockerHub](https://hub.docker.com/r/kpnnv/docker-rancher/).

### build image
```shell
$ make docker/build/<TAG>
```

### push image
```shell
$ make docker/push/<TAG>
```

### run rancher command
```shell
$ docker run --rm -v <PATH_TO_CONFIG>:/root/.rancher/cli2.json rancher:<TAG> "rancher --help"
```

### run helm command
```shell
$ docker run --rm rancher:<TAG> "helm --help"
```

### run kubectl command
```shell
$ docker run --rm -v <PATH_TO_CONFIG>:/root/.rancher/cli2.json rancher:<TAG> "rancher kubectl --help"
```

where `<TAG>` is the image tag and `<PATH_TO_CONFIG>` is the path for rancher client config path 

## Contributing

### Workflow
1. Fork this repository
2. Clone your fork
3. Create and test your changes
4. Create a pull-request
5. Wait for reviewers feedback

