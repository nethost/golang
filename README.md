# Golang Images

- development use *-ubuntu;
- production use *-alpine;
- alpine:3.8

## 1.x

```
$ docker build -t=nethost/golang:1.9-alpine .
$ docker push nethost/golang:1.9-alpine
$ docker pull nethost/golang:1.9-alpine

$ docker build -t=nethost/golang:1.10-alpine .
$ docker push nethost/golang:1.10-alpine
$ docker pull nethost/golang:1.10-alpine

$ docker build -t=nethost/golang:1.11-alpine .
$ docker push nethost/golang:1.11-alpine
$ docker pull nethost/golang:1.11-alpine
```

```
$ docker build -t=nethost/golang:1.9-ubuntu .
$ docker push nethost/golang:1.9-ubuntu
$ docker pull nethost/golang:1.9-ubuntu
```