# Hello World GHCR + Helm Example

This is a minimal example showing how to:

- Build a Docker image
- Push it to GitHub Container Registry (GHCR)
- Package a Helm chart
- Push the chart to GHCR as an OCI registry

## Setup

1. Replace `<OWNER>` in `charts/hello-world-public/values.yaml` with your GitHub username or organisation (lowercase).
2. Push this repo to GitHub.
3. Ensure Actions are enabled.
4. Push to the `main` branch or trigger the workflow manually.

The workflow will:

- Build and push `ghcr.io/<OWNER>/hello-world-public:latest`
- Package the Helm chart and push `hello-world-public` to `oci://ghcr.io/<OWNER>/charts`
