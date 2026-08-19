# AI Agent Studio Setup Guide

This guide summarizes setup paths verified from the included Dify-based source and documentation. AI Agent Studio requires buyer-managed infrastructure and third-party model/provider configuration.

## Minimum requirements stated upstream

- CPU: at least 2 cores.
- RAM: at least 4 GiB.
- Docker.
- Docker Compose v2.24.0 or newer for the Docker setup path.

## Docker setup path

The upstream quick-start uses the `docker/` directory and environment configuration. Because buyer packages exclude environment files and credentials, review the current upstream Dify Docker documentation and create your own environment configuration before starting services.

Typical Docker flow:

```powershell
cd docker
docker compose up -d
```

After services start, the upstream documentation points to `http://localhost/install` for first-time setup.

## Source development path

The included upstream API development documentation references:

- `uv`
- `pnpm`
- API, web and worker processes
- middleware services for local development

This path is intended for developers and requires careful local environment setup.

## Required buyer configuration

- Model provider accounts and API keys.
- Database, vector store, queue, storage and sandbox configuration.
- Network, TLS, backup and access-control decisions for production.

## Not verified

- One-click cloud deployment.
- Included API credits or hosted models.
- Guaranteed support for every AI provider.
- 15-minute setup.
- Production readiness without buyer-managed configuration and security review.
