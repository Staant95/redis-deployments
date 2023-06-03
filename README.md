# Run
```bash
docker compose up -d
```

## Test

### Secondary
```bash
docker exec -it secondary redis-cli -p 6389
> AUTH secret
> monitor
```
### Primary
```bash
docker exec -it primary redis-cli -p 6388
> AUTH secret
> SET foo bar
```

