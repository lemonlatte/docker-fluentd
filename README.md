# Docker Fluentd

## Build

```
$ docker build --rm=true -t docker-fluentd .
```

## Generate Config

```
$ docker run -it -v /docker/fluent:/fluent --entrypoint=/bin/bash docker-fluentd /setup.sh 
```

## Run

```
$ docker run -it -v /docker/fluent:/fluent docker-fluentd -c /fluent/fluent.conf
```
