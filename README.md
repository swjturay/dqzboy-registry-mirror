# Container Image Sync

Personal GitHub Actions workflows for mirroring selected container images to Aliyun ACR.

## Workflows

- [`sync-all-images-to-acr.yml`](.github/workflows/sync-all-images-to-acr.yml) mirrors the configured `linux/amd64` image set on a schedule or on demand.
- [`sync-image.yml`](.github/workflows/sync-image.yml) syncs one image on demand, for one platform or all architectures.
- [`sync-python-to-acr.yml`](.github/workflows/sync-python-to-acr.yml) syncs `python:3.12-slim` on demand.
- [`sync-sub-store-to-acr.yml`](.github/workflows/sync-sub-store-to-acr.yml) syncs `xream/sub-store:latest` on demand.

## Configuration

Add these repository Actions secrets:

- `ACR_USERNAME`
- `ACR_PASSWORD`

Image sources and destinations are configured directly in the workflow files.
