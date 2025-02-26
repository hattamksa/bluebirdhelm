# Bluebird Helm Chart

This Helm chart deploys a set of Kubernetes resources with optional components:

- **Service** (ClusterIP by default)
- **Deployment**
- **HPA** (disabled by default)
- **Ingress** (disabled by default, configured with `bluebird.deployment.id` host)
- **ConfigMap** (disabled by default, accepts custom key-value pairs)

## Installation

```sh
helm install my-release ./bluebird-chart
```

## Customization
Modify `values.yaml` to enable or disable specific components before deployment.

```sh
helm install my-release ./bluebird-chart -f values.yaml
```
