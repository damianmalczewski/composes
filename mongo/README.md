# Mongo Compose

Docker Compose configuration for MongoDB, deployed as single-note replica set.

Because initialization of replica set requires manual action, this prototype does it via separate single-job-purpose
container.

> [!IMPORTANT]
> The `mongo-init-job` is synchronized with main `mongo` container based on `healthcheck` and
> `condition: service_healthy`.

## Ports

| port    | info    |
| ------- | ------- |
| `27017` | MongoDB |
