# fg-docker-compose

# Description

This is a [Docker Compose](https://docs.docker.com/compose/) configuration which allows to start components of [FutureGateway](https://github.com/FutureGatewayFramework).

# Components

- `fgdb`: a `mariadb` based container which prepares database according to [fgapiserver_db.sql](https://github.com/FutureGatewayFramework/fgAPIServer/blob/master/fgapiserver_db.sql) file
- `fgapiserver`: an `eosc-fgapiserver` based container (see: [tzok/eosc-fgapiserver](https://github.com/tzok/eosc-fgapiserver))

# Usage

``` sh
docker-compose up
```

By default, this will launch `fgAPIServer` listening on port `8888` with an fresh database as defined in the upstream project.