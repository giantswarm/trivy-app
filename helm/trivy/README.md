# trivy

A Helm chart for trivy

**Homepage:** <https://github.com/giantswarm/trivy-app>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Giant Swarm applications team |  | <https://github.com/giantswarm/trivy-app> |

## Source Code

* <https://github.com/giantswarm/trivy-app>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
|  | trivy | 0.24.0 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| networkPolicy.enabled | bool | `true` |  |
| networkPolicy.ingress.namespaceSelector | object | `{}` |  |
| networkPolicy.ingress.podSelector | object | `{}` |  |
| ciliumNetworkPolicy.enabled | bool | `true` |  |
| verticalPodAutoscaler.trivy.enabled | bool | `true` |  |
| verticalPodAutoscaler.trivy.containerPolicies | object | `{}` |  |
| kyvernoPolicyExceptions.enabled | bool | `true` |  |
| kyvernoPolicyExceptions.namespace | string | `"giantswarm"` |  |
| trivy.rbac.pspEnabled | bool | `false` |  |
| trivy.image.registry | string | `"gsoci.azurecr.io"` |  |
| trivy.image.repository | string | `"giantswarm/trivy"` |  |
| trivy.securityContext.privileged | bool | `false` |  |
| trivy.securityContext.readOnlyRootFilesystem | bool | `true` |  |
| trivy.securityContext.allowPrivilegeEscalation | bool | `false` |  |
| trivy.trivy.dbRepository | string | `"gsoci.azurecr.io/giantswarm/trivy-db"` |  |
