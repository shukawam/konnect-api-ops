# Konnect APIOps

This is a demonstration for [APIOps](https://developer.konghq.com/deck/apiops/) using Kong Konnect.

## Pipeline overview

This sample provides a simple APIOps pipeline. The overview is as follows.

```mermaid
flowchart TD

A1[checkout] --> B1[setup inso] --> C1[setup deck] --> D1[lint openapi spec] --> E1[convert openapi to deck setting] --> F1[sync gateway setting]
```

## How to use

Set secret value to your repo.

```sh
gh secret set KONNECT_TOKEN --body "<your-konnect-token>"
gh secret set KONNECT_CONTROL_PLANE --body "<your-konnect-control-plane-name>"
```
