docker-noip2
============

* [build noip2 binary](build)
* build noip2 docker image

```
docker build -t tsaikd/noip2 .
```

* setup noip2 config

```
docker run -it --rm -v "${PWD}/etc:/usr/local/etc" tsaikd/noip2 -C
```

* docker-compose.yml

```
noip2:
  image: tsaikd/noip2
  volumes:
    - ./etc:/usr/local/etc
  stdin_open: true
  tty: true
```

