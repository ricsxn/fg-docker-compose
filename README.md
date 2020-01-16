# fg-docker-compose

# Description

This is a [Docker Compose](https://docs.docker.com/compose/) configuration which allows to start components of [FutureGateway](https://github.com/FutureGatewayFramework).

This work is co-funded by the [EOSC-hub project](http://eosc-hub.eu/) (Horizon 2020) under Grant number 777536.
<img src="https://wiki.eosc-hub.eu/download/attachments/1867786/eu%20logo.jpeg?version=1&modificationDate=1459256840098&api=v2" height="24">
<img src="https://wiki.eosc-hub.eu/download/attachments/18973612/eosc-hub-web.png?version=1&modificationDate=1516099993132&api=v2" height="24">

# Components

- `fgdb`: a `mariadb` based container which prepares database according to [fgapiserver_db.sql](https://github.com/FutureGatewayFramework/fgAPIServer/blob/master/fgapiserver_db.sql) file
- `fgapiserver`: an `eosc-fgapiserver` based container (see: [tzok/eosc-fgapiserver](https://github.com/tzok/eosc-fgapiserver))

# Usage

``` sh
docker-compose up
```

By default, this will launch `fgAPIServer` listening on port `8888` with an fresh database as defined in the upstream project.
