# mariadb-instance

![Version: 0.29.3](https://img.shields.io/badge/Version-0.29.3-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.29.0](https://img.shields.io/badge/AppVersion-0.29.0-informational?style=flat-square)

A Helm chart to stand up a mariadb instance

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| database | string | `"mariadb"` | Application database name |
| metrics.enabled | bool | `true` | Whether to enable Prometheus metrics |
| name | string | `"mariadb"` | Name of the mariadb instance |
| port | int | `3306` | Port to expose the service on |
| rootPasswordSecret.generate | bool | `true` | Whether to autogenerate the password |
| rootPasswordSecret.key | string | `"password"` | Key within the secret |
| rootPasswordSecret.name | string | `"mariadb-root"` | Name of the secret to store the root password |
| service.type | string | `"ClusterIP"` | Service type |
| storage.size | string | `"1Gi"` | Amount of storage to assign to the PVC |
| storage.storageClassName | string | `""` | Storage class name |
| userPasswordSecret.generate | bool | `true` | Whether to autogenerate the password |
| userPasswordSecret.key | string | `"password"` | Key within the secret |
| userPasswordSecret.name | string | `"mariadb-password"` | Name of the secret to store the root password |
| username | string | `"mariadb"` | Application username to assign to the instance |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.14.2](https://github.com/norwoodj/helm-docs/releases/v1.14.2)
