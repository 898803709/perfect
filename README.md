# perfect

## build 

```
docker build -t prefect-docker-guide-image .
```

## up
```
docker run --network="host" -e PREFECT_API_URL=http://host.docker.internal:4200/api prefect-docker-guide-image
```

## start service
```
poetry run prefect server start
```

## コンテナに入る
```
docker-compose run --rm -it prefect bash
```