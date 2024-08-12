# SnipeIT

## Usage

### Start the container

```bash
docker compose up -d
```

Open the browser and go to `http://localhost:8080`. 
To get access to the mailhog, go to `http://localhost:8025`.

### Restart the container

```bash
docker compose down && docker compose up -d
```

## Generatw App Key

```bash
docker compose run --rm app php artisan key:generate --show
```

## Experimental

### Send a test email with mailhog

```bash
docker compose run --rm mailhog /usr/sbin/sendmail -S mail:1025
```
