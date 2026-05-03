# Docker host networking

Minimal example: a static site served by Python’s built-in HTTP server with `network_mode: host` in Docker Compose.

## What this demonstrates

The container shares the host’s network stack (primarily on **Linux**). The app listens on **port 8888** on the host itself. You do not use `ports:` mappings with host networking; publishing is implicit.

## Deploy with Coolify

Use the [root README](../README.md) flow with:

- **Base Directory:** `/host-network`
- **Docker Compose Location:** `/compose.yaml`

In the Configuration > General tab > Build section ensure "Preserve Repository During Deployment" is checked.
Without this, the `public` directory won't be available to the container.