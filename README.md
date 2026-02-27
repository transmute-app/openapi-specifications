# openapi-specifications

This repository is **fully automated** and managed by GitHub actions workflows. Its contents should not be edited manually.

## Purpose

This repository acts as a CDN layer for serving OpenAPI specifications directly from the transmute.sh website. By decoupling the specs from the main source code, we avoid any impact on existing CI/CD pipelines or development workflows.

## How it works

- OpenAPI specifications are published to this repository automatically on commit to main in [transmute-app/transmute](https://github.com/transmute-app/transmute).
- The specs are served directly from this repository via GitHub's raw content delivery, making them accessible at stable, predictable URLs.
- No manual intervention is required — all updates are handled by automation.

## Do not edit manually

Changes pushed directly to this repository may be overwritten by the next automated update. If you need to modify an OpenAPI specification, make the change in the originating source repository and let the automation propagate it here.

## URLs

Specs served from this repository are available at:

```
https://raw.githubusercontent.com/transmute-app/openapi-specifications/main/openapi.json
```
