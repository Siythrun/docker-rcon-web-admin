
This image lets you run the [rcon-web-admin](https://github.com/lacaulac/rcon-web-admin) administration tool as a
Docker container. A great benefit of runnings rcon-web-admin in Docker, especially
in a Docker Swarm or Composition is that the RCON port of your game server
can remain securely isolated within the Docker network.

## Getting Started

To get up and running quickly, use

```
docker run -d -v /srv/rcon-web-admin:/opt/rcon-web-admin/db  -p 4326:4326 -p 4327:4327 siythrun/rcon
```

With that you can follow the [regular instructions](https://github.com/brainfoolong/rcon-web-admin#open-in-browser) and
access the web UI at http://YOUR_DOCKER_HOST:4326

## Options

### VOLUMEs

* /opt/rcon-web-admin/db

### PORTs

* 4326 : web UI
* 4327 : websocket access from UI

## Examples
