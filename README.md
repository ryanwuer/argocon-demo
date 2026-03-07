# argocon-demo

A minimal Helm chart demonstrating an Argo Rollouts canary rollout for Argo CD demos.

## Included

- `Helm` chart named `argocon-demo`
- `Argo Rollout` custom resource
- Canary steps:
  - `10%`
  - `pause`
  - `50%`
  - `pause`
  - `100%`
- `replicas: 10`

## Render

```bash
helm template argocon-demo ./chart
```

## Install

```bash
helm upgrade --install argocon-demo ./chart
```
