FROM postgres:13.14-alpine3.19

COPY . /docker-entrypoint-initdb.d

ENV POSTGRES_DB="oracion"
ENV POSTGRES_USER="gaston"
ENV POSTGRES_PASSWORD="gaston"