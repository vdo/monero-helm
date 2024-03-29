# monero-helm

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v0.18.2.0](https://img.shields.io/badge/AppVersion-v0.18.2.0-informational?style=flat-square)

A Helm chart for Monero node

**Homepage:** <https://getmonero.org/>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| vdo 1138 | <vdo1138@rbx.run> |  |

## Source Code

* <https://github.com/vdo/monero-chart>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `10` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| cluster | string | `"monero"` |  |
| config.network | string | `nil` |  |
| config.prune | bool | `false` |  |
| config.zmq | bool | `true` |  |
| container.ports.p2p | int | `31080` |  |
| container.ports.rpc | int | `18081` |  |
| container.ports.rpcrestricted | int | `18089` |  |
| container.ports.zmq | int | `18082` |  |
| container.ports.zmqpub | int | `18083` |  |
| fullnameOverride | string | `""` |  |
| image.args | list | `[]` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"sethsimmons/simple-monerod"` |  |
| image.tag | string | `"v0.18.2.0"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.enabled | bool | `false` |  |
| labels | object | `{}` |  |
| nameOverride | string | `""` |  |
| persistence.accessModes[0] | string | `"ReadWriteOnce"` |  |
| persistence.annotations | object | `{}` |  |
| persistence.enabled | bool | `true` |  |
| persistence.size | string | `"150Gi"` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext.fsGroup | int | `1000` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext.runAsNonRoot | bool | `true` |  |
| securityContext.runAsUser | int | `1000` |  |
| service.rpc | int | `18081` |  |
| service.rpcrestricted | int | `18089` |  |
| service.type | string | `"ClusterIP"` |  |
| service.zmq | int | `18082` |  |
| service.zmqpub | int | `18083` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `""` |  |
| serviceP2P.p2p | int | `31080` |  |
| serviceP2P.type | string | `"NodePort"` |  |
| tolerations | list | `[]` |  |
| volumes.data.mountPath | string | `"/home/monero/.bitmonero"` |  |

----------------------------------------------
## License

See [LICENSE](LICENSE.txt)
