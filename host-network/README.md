# Docker host networking

Minimal example: a static site served by Python’s built-in HTTP server with `network_mode: host` in Docker Compose.

## What this demonstrates

The container shares the host’s network stack (primarily on **Linux**). The app listens on **port 8888** on the host itself. You do not use `ports:` mappings with host networking; publishing is implicit.

On **Docker Desktop** (macOS and Windows), host networking does not behave like it does on Linux. Use a Linux server or VM for a faithful test.

## Run locally

From this directory:

```bash
docker compose up
```

Open [http://localhost:8888](http://localhost:8888) (on Linux). Content is served from `./public`.

## Deploy with Coolify

Use the [root README](../README.md) flow with:

- **Base Directory:** `/host-network`
- **Docker Compose Location:** `/compose.yaml`

If your platform routes traffic through a reverse proxy that expects standard Docker bridge port publishing, you may need extra host firewall or routing configuration for host-mode services.
