# docker-webdis

## Usage

```sh
wget https://github.com/yongjhih/docker-webdis/raw/master/docker-compose.yml
docker-compose up
```

* host:webdis:7379
* guest:redis:6379

## Testing

```sh
curl http://127.0.0.1:7379/SET/hello/world
```

## Credit

* https://github.com/anapsix/docker-webdis
