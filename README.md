# Coolify Example Apps

A collection of example apps for deploying to Coolify.

## Deploying with Coolify

1. Projects > <Project Name> >Add Resource
2. Select "Public Repository
3. For Repository URL enter:
    ```
    https://github.com/r-portas/coolify-example-apps
    ```
4. For app config enter:
    - Base Directory: `/<app-name>
    - Docker Compose Location: `/compose.yaml` (Note the leading slash is important)
    - Click "Continue
5. In the general tab:
    - Name: `<app-name>`
    - Click "Save"
    - Click "Deploy"

## Apps

- [UpTime Kuma](./uptime-kuma)