# Docker Sandbox Env

## Config
map docker ip with `api.docker-local.com` and `interface.docker-local.com`

## Folder structure
```
|- config/
|  |- reverse-proxy/
|  |  |- api-service.conf
|  |  |- interface-service.conf
|- data/
|- images/
|  |- reverse-proxy/Dockerfile.php
|- src/
|  |- api-service/index.php
|  |- interface-service/index.php
```

## Reverse proxy
to use reverse proxy (nginx)
- not expose port in application data
- links application container with reverse-proxy container
