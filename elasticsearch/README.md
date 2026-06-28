# Elasticsearch Compose

Docker Compose configuration for [Elasticsearch](https://www.elastic.co/elasticsearch), deployed as a single-node
cluster with security disabled. Includes [Elasticvue](https://elasticvue.com/) as a web UI.

## Ports

| port   | info                    |
|--------|-------------------------|
| `9200` | Elasticsearch HTTP API  |
| `9300` | Elasticsearch transport |
| `9201` | Elasticvue web UI       |
