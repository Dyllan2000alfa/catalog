# netbootxyz

![Version: 0.0.5](https://img.shields.io/badge/Version-0.0.5-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.6.6](https://img.shields.io/badge/AppVersion-0.6.6-informational?style=flat-square)

Netbootxyz App for TrueNAS SCALE

**Homepage:** <https://github.com/truecharts/apps/tree/master/charts/stable/netbootxyz>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| TrueCharts | info@truecharts.org | https://truecharts.org |

## Source Code

* <https://github.com/truecharts/apps/tree/master/charts/netbootxyz>

## Requirements

Kubernetes: `>=1.16.0-0`

| Repository | Name | Version |
|------------|------|---------|
| https://truecharts.org | common | 8.15.4 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| env | object | `{}` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/netbootxyz/netbootxyz"` |  |
| image.tag | string | `"0.6.6-nbxyz10@sha256:4fff0c570ba97c1640ab86e61111920505389c0f42e2645b0ff4d4b3e742e594"` |  |
| persistence.assets.enabled | bool | `true` |  |
| persistence.assets.mountPath | string | `"/assets"` |  |
| persistence.config.enabled | bool | `true` |  |
| persistence.config.mountPath | string | `"/config"` |  |
| podSecurityContext.runAsGroup | int | `0` |  |
| podSecurityContext.runAsUser | int | `0` |  |
| securityContext.readOnlyRootFilesystem | bool | `false` |  |
| securityContext.runAsNonRoot | bool | `false` |  |
| service.assets.enabled | bool | `true` |  |
| service.assets.ports.assets.enabled | bool | `true` |  |
| service.assets.ports.assets.port | int | `10162` |  |
| service.assets.ports.assets.targetport | int | `80` |  |
| service.main.ports.main.port | int | `10161` |  |
| service.main.ports.main.targetPort | int | `3000` |  |
| service.tftp.enabled | bool | `true` |  |
| service.tftp.ports.tftp.enabled | bool | `true` |  |
| service.tftp.ports.tftp.port | int | `69` |  |
| service.tftp.ports.tftp.protocol | string | `"UDP"` |  |
| service.tftp.ports.tftp.targetport | int | `69` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
