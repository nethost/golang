# Golang Images

- development use *-ubuntu;
- production use *-alpine;
- alpine:3.8

## 1.9

```
$ docker build -t=nethost/golang:1.9-alpine .
$ docker push nethost/golang:1.9-alpine
$ docker pull nethost/golang:1.9-alpine

$ docker build -t=nethost/golang:1.9-ubuntu .
$ docker push nethost/golang:1.9-ubuntu
$ docker pull nethost/golang:1.9-ubuntu
```