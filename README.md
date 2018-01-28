# Postgres for Docker with locale de_DE.UTF-8

[![Docker Build Status](https://img.shields.io/docker/build/shelvis/postgres.svg)](https://hub.docker.com/r/shelvis/postgres-docker/builds/)

This is a customized docker build with german localization.

```
FROM postgres:latest
RUN localedef -i de_DE -c -f UTF-8 -A /usr/share/locale/locale.alias de_DE.UTF-8
ENV LANG de_DE.utf8
```