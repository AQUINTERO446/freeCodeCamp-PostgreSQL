# Postgres
## Instalation
### Docker Run

```
docker network create -d bridge some-network

docker run --name some-postgres \
    -e POSTGRES_PASSWORD=mysecretpassword \
    --network some-network \
    -p 5432:5432 \
    -d postgres:11.0

```
### Docker Compose
```
docker-compose up -d
```

## Connect to Database
```
docker run -it --rm \
    --network postgres-onboarding_default \
    postgres:11.0 \
    psql -h some-postgres -U postgres -W
```

## Client Options
* [DBeaver](https://dbeaver.io/)
* [TablePlus](https://tableplus.com/)
