# netbox-compose

My [Netbox](https://netboxlabs.com/products/netbox/) docker compose files. I borrowed alot of the content from the [Netbox docker github repo](https://github.com/netbox-community/netbox-docker)

## .env example

```bash
NETBOX_VERSION=version
POSTGRES_VERSION=version
REDIS_VERSION=version
```

## netbox.env example

SECRET_KEY must be at least 50 characters in length, and should contain a mix of letters, digits, and symbols. The script located at $INSTALL_ROOT/netbox/generate_secret_key.py may be used to generate a suitable key.

```bash
CORS_ORIGIN_ALLOW_ALL=True
DB_HOST=postgres
DB_NAME=netbox
DB_PASSWORD=password
DB_USER=netbox
EMAIL_FROM=mail@domain.com
EMAIL_PASSWORD=password
EMAIL_PORT=25
EMAIL_SERVER=localhost
EMAIL_SSL_CERTFILE=path
EMAIL_SSL_KEYFILE=path
EMAIL_TIMEOUT=5
EMAIL_USERNAME=netbox
# EMAIL_USE_SSL and EMAIL_USE_TLS are mutually exclusive, i.e. they can't both be `true`!
EMAIL_USE_SSL=false
EMAIL_USE_TLS=false
GRAPHQL_ENABLED=true
MEDIA_ROOT=/opt/netbox/netbox/media
METRICS_ENABLED=false
REDIS_CACHE_DATABASE=1
REDIS_CACHE_HOST=redis-cache
REDIS_CACHE_INSECURE_SKIP_TLS_VERIFY=false
REDIS_CACHE_PASSWORD=password
REDIS_CACHE_SSL=false
REDIS_DATABASE=0
REDIS_HOST=redis
REDIS_INSECURE_SKIP_TLS_VERIFY=false
REDIS_PASSWORD=password
REDIS_SSL=false
RELEASE_CHECK_URL=https://api.github.com/repos/netbox-community/netbox/releases
SECRET_KEY=key
SKIP_SUPERUSER=true
WEBHOOKS_ENABLED=true
```

## postgres.env example

```bash
POSTGRES_DB=netbox
POSTGRES_PASSWORD=password
POSTGRES_USER=netbox
```

## redis.env example

```bash
REDIS_PASSWORD=password
```

## redis-cache.env example

```bash
REDIS_PASSWORD=password
```
