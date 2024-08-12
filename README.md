# SnipeIT

## Usage

### Start the container

```bash
docker compose up -d
```

- Open the browser and go to `http://localhost:8080`. 
- To get access to the mailhog, go to `http://localhost:8025`.

### Restart the container

```bash
docker compose down && docker compose up -d
```

### Generate app key

```bash
docker compose run --rm app php artisan key:generate --show
```
