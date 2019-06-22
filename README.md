Hello World
===========

This is a simple Docker image that just gives http responses on port 8000.

```bash
$ docker images | grep hell
REPOSITORY               TAG       IMAGE ID        CREATED          VIRTUAL SIZE
crccheck/hello-world     latest    2b28c6ad8d1b    4 months ago     1.2MB
```


Sample Usage
------------

### Starting a web server on port 80

```bash
$ docker run -d --rm --name web-test -p 80:8000 crccheck/hello-world
```

You can now interact with this as if it were a dumb web server:

```
$ curl localhost
```
