FROM alpine:3.8
LABEL maintainer="Billgo <cocobill@vip.qq.com>"

ENV GO_VERSION 1.9.2

RUN apk update && \
    apk upgrade && \
    apk add --no-cache ca-certificates tzdata bash && \
    ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone && \
    mkdir -p /etc/BUILDS/ && \
    printf "Build of nethost/golang, date: %s\n"  `date -u +"%Y-%m-%dT%H:%M:%SZ"` > /etc/BUILDS/golang && \
    apk add curl && \
    curl https://storage.googleapis.com/golang/go$GO_VERSION.linux-amd64.tar.gz | tar xzf - -C / && \
    mv /go /goroot && \
    apk del curl && \
    rm -rf /var/cache/apk/*

ENV GOROOT=/goroot \
    GOPATH=/gopath \
    GOBIN=/gopath/bin \
    PATH=${PATH}:/goroot/bin:/gopath/bin