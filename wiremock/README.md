# WireMock

[WireMock](https://wiremock.org/) HTTP mock server for API stubbing and testing.

Stub mappings go in `wiremock/mappings/`, static response files in `wiremock/__files/`. Both directories are mounted read-only.

Includes a sample stub: `GET /hello` → `200 {"message": "hello world"}`.

## Ports

| port   | info            |
|--------|-----------------|
| `1080` | HTTP mock / API |
