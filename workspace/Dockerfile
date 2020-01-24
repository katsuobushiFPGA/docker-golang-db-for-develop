FROM golang:1.13.6-alpine

WORKDIR /go/src/app

ENV GO111MODULE=on
RUN apk add --no-cache \
    bash \
    alpine-sdk \
    git \
    && go get github.com/pilu/fresh
