# docker-webdis

[![Deploy to Docker Cloud](https://github.com/yongjhih/docker-parse-server/raw/master/art/deploy-to-docker-cloud.png)](https://stackfiles.io/registry/56ca423523bc9401006b5acb)

## Usage

```sh
wget https://github.com/yongjhih/docker-webdis/raw/master/docker-compose.yml
docker-compose up
```

* host:webdis:7379
* guest:redis:6379

## Configuration

environment:

- THREADS
- POOL_SIZE
- WEBSOCKETS
- ACL_DISABLED
- ACL_HTTP_BASIC_AUTH
- ACL_HTTP_BASIC_AUTH_ENABLED
- VERBOSITY
- LOGFILE
- DATABASE
- REDIS_HOST
- REDIS_PORT
- REDIS_AUTH

volumes:

- '$PWD/webdis.log:/webdis.log'

## Testing

```sh
curl http://127.0.0.1:7379/SET/hello/world
```

## Credit

* https://github.com/anapsix/docker-webdis
