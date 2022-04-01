FROM mongo

LABEL maintainer="bonsai-team"
LABEL project="microservices"

ENV MONGO_INITDB_DATABASE="users"
ENV MONGO_INITDB_ROOT_USERNAME="admin"
ENV MONGO_INITDB_ROOT_PASSWORD="root"

RUN mkdir -p /data/db
VOLUME [ "/data/db", "/data/configdb" ]

COPY ./init-mongodb.sh /docker-entrypoint-initdb.d