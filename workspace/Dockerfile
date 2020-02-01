FROM golang:1.13.6-alpine

WORKDIR /go/src/app

ENV GO111MODULE=on
RUN apk add --no-cache \
    bash \
    alpine-sdk \
    git \
    sqlite \
    && go get github.com/pilu/fresh

RUN apk --update add tzdata && \
    cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime && \
    apk del tzdata && \
    rm -rf /var/cache/apk/*