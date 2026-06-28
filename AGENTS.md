# Agent Instructions

## `docker-compose.yaml` - service key ordering

Keys inside each service block must follow this order:

1. `image`
2. `ports`
3. `environment`
4. `entrypoint`
5. `command`
6. `volumes`
7. `networks`
8. `healthcheck`
9. `depends_on`
10. `restart`

Keys not in this list (e.g. `security_opt`, `profiles`) go immediately after the last key from the list above and are 
sorted alphanumerically.

## `dependabot.yml`

- Entries sorted alphabetically by `directory`.
- Every entry includes a `groups` block with `patterns: ["*"]` so all image bumps in a directory land in one PR.
- `open-pull-requests-limit: 1` on every entry.
- Every compose directory from the public Docker registry must have a corresponding entry.

## `README.md`

Each compose directory must have a `README.md` with:

- H1 title (service name)
- Short description with a link to the image or project page
- `## Ports` section - a Markdown table with `port` and `info` columns
