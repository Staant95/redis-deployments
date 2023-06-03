# Description
A volume is created for the redis data. The redis server is configured to use the volume.
## Run
```bash
docker compose up -d
```

## Test
```bash
docker exec -it redis-stack-server redis-cli
> SET foo bar
```

