# Generic Helm Chart


A generic Helm chart for application Deployments. With this chart you can role out deployment, service, ingress and many more manifest files at once.

For examples and other tips please have look at the default `values.yaml`.

## The following features are currently supported:
- Service + Ingress object creation (with TLS)
- Service Account creation
- PVC and Volume Management
- Features for Deployments:
    - configure env vars
    - create env from secrets
    - configure probes
    - configure volumes and mounts (also from secrets)
    - horizontal pod scaling
    - sidecar injection
    - node selection
    - define deployment strategy (since v0.6.0)
- sealed secrets

## Limitations
- currently, only one ingress and host per app is supported
- No support for cronjobs
