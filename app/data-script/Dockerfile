# syntax=docker/dockerfile:1

FROM alpine

WORKDIR /opt

COPY import.sh mydatabase.sql ./

RUN apk update && apk add --no-cache mysql-client

CMD sh import.sh