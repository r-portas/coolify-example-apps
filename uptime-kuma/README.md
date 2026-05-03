# Uptime Kuma

Example deployment of [Uptime Kuma](https://github.com/louislam/uptime-kuma) via Docker Compose, with a persistent volume for application data.

## Service

- **Image:** `louislam/uptime-kuma:2`
- **Port:** `3001` (mapped `3001:3001` on the host)
- **Volume:** `uptime-kuma-data` mounted at `/app/data`

The `DUMMY_TEST_VAR` environment variable in `compose.yaml` is a placeholder; remove or replace it with real configuration as needed.

## Deploy with Coolify

Use the [root README](../README.md) flow with:

- **Base Directory:** `/uptime-kuma`
- **Docker Compose Location:** `/compose.yaml`