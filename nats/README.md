# NATS Compose

Compose setup for [NATS](https://docs.nats.io/).

## Ports

| port   | info                                      |
| ------ | ----------------------------------------- |
| `4222` | Client connections (publish/subscribe)    |
| `8222` | Monitoring and health checks (`/healthz`) |
| `6222` | Cluster node communication                |
