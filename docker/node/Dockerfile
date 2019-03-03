FROM node:10.15.2-alpine

WORKDIR /srv

RUN apk update && apk upgrade
RUN apk add --no-cache alpine-sdk \
    bash \
    tzdata
