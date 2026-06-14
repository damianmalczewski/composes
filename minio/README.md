# Minio Compose

Docker Compose configuration for [MinIO](https://github.com/minio/minio). Provides two sandbox
setups - a standalone one and a `minio-cluster` (with 4 replicas and reverse proxy).

## Ports

| port   | info    |
| ------ | ------- |
| `9000` | S3 API  |
| `9001` | Console |
