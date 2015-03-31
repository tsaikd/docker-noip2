How to build noip2 binary
=========================

* build noip2 binary from docker image

```
docker build -t tsaikd/docker-noip2:build .
```

* copy noip2 binary from docker image

```
docker run -it --rm -v ${PWD}:/usr/local/bin tsaikd/docker-noip2:build
```

