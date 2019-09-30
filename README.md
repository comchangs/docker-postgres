Chan# **postgres**
___

### Description

This image runs [*PostgreSQL*](https://www.postgresql.org/) on a Debian Jessie Linux distribution.

The image extends the official [*PostgreSQL*](https://hub.docker.com/_/postgres/) one, adding the support for:

 * the [*Debezium Postgres Decoderbufs*](https://github.com/debezium/postgres-decoderbufs.git) plugin

The *latest* tag of this image is build with the [latest stable](https://www.postgresql.org/) release of PostgreSQL.

You can pull it with:

    docker pull comchangs/postgres


You can also find other images based on different PostgreSQL releases, using a different tag in the following form:

    docker pull comchangs/postgres:[postgres-release]


For example, if you want the latest PostgreSQL major release 9.5 (actually 9.5.7) you can pull the image with:

    docker pull comchangs/postgres:9.5

Run with Docker Compose:

    docker-compose -p comchangs up

Setting the project name to *parrot* with the **-p** option is useful to share the network created with the containers coming from other Parrot docker-compose.yml configurations.

You can access PostgreSql using:

    hostname: localhost
    port:     5432
    username: postgres
    password: postgres

