# Demonstrating the power of Compose Include


## Pre-requisite

- Install Docker Compose v2.20.x

```
  wget https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-x86_64
  mv docker-compose-linux-x86_64 docker-compose
  chmod +x docker-compose
```

```
  docker-compose version
  Docker Compose version v2.20.2
```

## Getting Started

## Clone the repository

```
 git clone https://github.com/ajeetraina/compose-include/
 cd compose-include
```

## Run the Services

```
 docker-compose -f web.yaml up
```

```
docker-compose -f web.yaml ps 
NAME                IMAGE               COMMAND                  SERVICE             CREATED             STATUS              PORTS
root-database-1     postgres:12         "docker-entrypoint.s…"   database            10 minutes ago      Up 2 minutes        5432/tcp
root-web-1          nginx:latest        "/docker-entrypoint.…"   web                 10 minutes ago      Up 2 minutes        80/tcp
```
