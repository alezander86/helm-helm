# postgresql

![Version: 12.2.6](https://img.shields.io/badge/Version-12.2.6-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 15.2.0](https://img.shields.io/badge/AppVersion-15.2.0-informational?style=flat-square)

PostgreSQL (Postgres) is an open source object-relational database known for reliability and data integrity. ACID-compliant, it supports foreign keys, joins, views, triggers and stored procedures.

**Homepage:** <https://github.com/bitnami/charts/tree/main/bitnami/postgresql>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Bitnami |  | <https://github.com/bitnami/charts> |

## Source Code

* <https://github.com/bitnami/containers/tree/main/bitnami/postgresql>
* <https://www.postgresql.org/>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://charts.bitnami.com/bitnami | common | 2.x.x |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| architecture | string | `"standalone"` |  |
| audit.clientMinMessages | string | `"error"` |  |
| audit.logConnections | bool | `false` |  |
| audit.logDisconnections | bool | `false` |  |
| audit.logHostname | bool | `false` |  |
| audit.logLinePrefix | string | `""` |  |
| audit.logTimezone | string | `""` |  |
| audit.pgAuditLog | string | `""` |  |
| audit.pgAuditLogCatalog | string | `"off"` |  |
| auth.database | string | `""` |  |
| auth.enablePostgresUser | bool | `true` |  |
| auth.existingSecret | string | `""` |  |
| auth.password | string | `""` |  |
| auth.postgresPassword | string | `""` |  |
| auth.replicationPassword | string | `""` |  |
| auth.replicationUsername | string | `"repl_user"` |  |
| auth.secretKeys.adminPasswordKey | string | `"postgres-password"` |  |
| auth.secretKeys.replicationPasswordKey | string | `"replication-password"` |  |
| auth.secretKeys.userPasswordKey | string | `"password"` |  |
| auth.usePasswordFiles | bool | `false` |  |
| auth.username | string | `""` |  |
| clusterDomain | string | `"cluster.local"` |  |
| commonAnnotations | object | `{}` |  |
| commonLabels | object | `{}` |  |
| containerPorts.postgresql | int | `5432` |  |
| diagnosticMode.args[0] | string | `"infinity"` |  |
| diagnosticMode.command[0] | string | `"sleep"` |  |
| diagnosticMode.enabled | bool | `false` |  |
| extraDeploy | list | `[]` |  |
| fullnameOverride | string | `""` |  |
| global.imagePullSecrets | list | `[]` |  |
| global.imageRegistry | string | `""` |  |
| global.postgresql.auth.database | string | `""` |  |
| global.postgresql.auth.existingSecret | string | `""` |  |
| global.postgresql.auth.password | string | `""` |  |
| global.postgresql.auth.postgresPassword | string | `""` |  |
| global.postgresql.auth.secretKeys.adminPasswordKey | string | `""` |  |
| global.postgresql.auth.secretKeys.replicationPasswordKey | string | `""` |  |
| global.postgresql.auth.secretKeys.userPasswordKey | string | `""` |  |
| global.postgresql.auth.username | string | `""` |  |
| global.postgresql.service.ports.postgresql | string | `""` |  |
| global.storageClass | string | `""` |  |
| image.debug | bool | `false` |  |
| image.digest | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.pullSecrets | list | `[]` |  |
| image.registry | string | `"docker.io"` |  |
| image.repository | string | `"bitnami/postgresql"` |  |
| image.tag | string | `"15.2.0-debian-11-r14"` |  |
| kubeVersion | string | `""` |  |
| ldap.basedn | string | `""` |  |
| ldap.binddn | string | `""` |  |
| ldap.bindpw | string | `""` |  |
| ldap.enabled | bool | `false` |  |
| ldap.port | string | `""` |  |
| ldap.prefix | string | `""` |  |
| ldap.scheme | string | `""` |  |
| ldap.searchAttribute | string | `""` |  |
| ldap.searchFilter | string | `""` |  |
| ldap.server | string | `""` |  |
| ldap.suffix | string | `""` |  |
| ldap.tls.enabled | bool | `false` |  |
| ldap.uri | string | `""` |  |
| metrics.containerPorts.metrics | int | `9187` |  |
| metrics.containerSecurityContext.enabled | bool | `true` |  |
| metrics.containerSecurityContext.runAsNonRoot | bool | `true` |  |
| metrics.containerSecurityContext.runAsUser | int | `1001` |  |
| metrics.customLivenessProbe | object | `{}` |  |
| metrics.customMetrics | object | `{}` |  |
| metrics.customReadinessProbe | object | `{}` |  |
| metrics.customStartupProbe | object | `{}` |  |
| metrics.enabled | bool | `false` |  |
| metrics.extraEnvVars | list | `[]` |  |
| metrics.image.digest | string | `""` |  |
| metrics.image.pullPolicy | string | `"IfNotPresent"` |  |
| metrics.image.pullSecrets | list | `[]` |  |
| metrics.image.registry | string | `"docker.io"` |  |
| metrics.image.repository | string | `"bitnami/postgres-exporter"` |  |
| metrics.image.tag | string | `"0.12.0-debian-11-r71"` |  |
| metrics.livenessProbe.enabled | bool | `true` |  |
| metrics.livenessProbe.failureThreshold | int | `6` |  |
| metrics.livenessProbe.initialDelaySeconds | int | `5` |  |
| metrics.livenessProbe.periodSeconds | int | `10` |  |
| metrics.livenessProbe.successThreshold | int | `1` |  |
| metrics.livenessProbe.timeoutSeconds | int | `5` |  |
| metrics.prometheusRule.enabled | bool | `false` |  |
| metrics.prometheusRule.labels | object | `{}` |  |
| metrics.prometheusRule.namespace | string | `""` |  |
| metrics.prometheusRule.rules | list | `[]` |  |
| metrics.readinessProbe.enabled | bool | `true` |  |
| metrics.readinessProbe.failureThreshold | int | `6` |  |
| metrics.readinessProbe.initialDelaySeconds | int | `5` |  |
| metrics.readinessProbe.periodSeconds | int | `10` |  |
| metrics.readinessProbe.successThreshold | int | `1` |  |
| metrics.readinessProbe.timeoutSeconds | int | `5` |  |
| metrics.resources.limits | object | `{}` |  |
| metrics.resources.requests | object | `{}` |  |
| metrics.service.annotations."prometheus.io/port" | string | `"{{ .Values.metrics.service.ports.metrics }}"` |  |
| metrics.service.annotations."prometheus.io/scrape" | string | `"true"` |  |
| metrics.service.clusterIP | string | `""` |  |
| metrics.service.ports.metrics | int | `9187` |  |
| metrics.service.sessionAffinity | string | `"None"` |  |
| metrics.serviceMonitor.enabled | bool | `false` |  |
| metrics.serviceMonitor.honorLabels | bool | `false` |  |
| metrics.serviceMonitor.interval | string | `""` |  |
| metrics.serviceMonitor.jobLabel | string | `""` |  |
| metrics.serviceMonitor.labels | object | `{}` |  |
| metrics.serviceMonitor.metricRelabelings | list | `[]` |  |
| metrics.serviceMonitor.namespace | string | `""` |  |
| metrics.serviceMonitor.relabelings | list | `[]` |  |
| metrics.serviceMonitor.scrapeTimeout | string | `""` |  |
| metrics.serviceMonitor.selector | object | `{}` |  |
| metrics.startupProbe.enabled | bool | `false` |  |
| metrics.startupProbe.failureThreshold | int | `15` |  |
| metrics.startupProbe.initialDelaySeconds | int | `10` |  |
| metrics.startupProbe.periodSeconds | int | `10` |  |
| metrics.startupProbe.successThreshold | int | `1` |  |
| metrics.startupProbe.timeoutSeconds | int | `1` |  |
| nameOverride | string | `""` |  |
| networkPolicy.egressRules.customRules | object | `{}` |  |
| networkPolicy.egressRules.denyConnectionsToExternal | bool | `false` |  |
| networkPolicy.enabled | bool | `false` |  |
| networkPolicy.ingressRules.primaryAccessOnlyFrom.customRules | object | `{}` |  |
| networkPolicy.ingressRules.primaryAccessOnlyFrom.enabled | bool | `false` |  |
| networkPolicy.ingressRules.primaryAccessOnlyFrom.namespaceSelector | object | `{}` |  |
| networkPolicy.ingressRules.primaryAccessOnlyFrom.podSelector | object | `{}` |  |
| networkPolicy.ingressRules.readReplicasAccessOnlyFrom.customRules | object | `{}` |  |
| networkPolicy.ingressRules.readReplicasAccessOnlyFrom.enabled | bool | `false` |  |
| networkPolicy.ingressRules.readReplicasAccessOnlyFrom.namespaceSelector | object | `{}` |  |
| networkPolicy.ingressRules.readReplicasAccessOnlyFrom.podSelector | object | `{}` |  |
| networkPolicy.metrics.enabled | bool | `false` |  |
| networkPolicy.metrics.namespaceSelector | object | `{}` |  |
| networkPolicy.metrics.podSelector | object | `{}` |  |
| postgresqlDataDir | string | `"/bitnami/postgresql/data"` |  |
| postgresqlSharedPreloadLibraries | string | `"pgaudit"` |  |
| primary.affinity | object | `{}` |  |
| primary.annotations | object | `{}` |  |
| primary.args | list | `[]` |  |
| primary.command | list | `[]` |  |
| primary.configuration | string | `""` |  |
| primary.containerSecurityContext.enabled | bool | `true` |  |
| primary.containerSecurityContext.runAsUser | int | `1001` |  |
| primary.customLivenessProbe | object | `{}` |  |
| primary.customReadinessProbe | object | `{}` |  |
| primary.customStartupProbe | object | `{}` |  |
| primary.existingConfigmap | string | `""` |  |
| primary.existingExtendedConfigmap | string | `""` |  |
| primary.extendedConfiguration | string | `""` |  |
| primary.extraEnvVars | list | `[]` |  |
| primary.extraEnvVarsCM | string | `""` |  |
| primary.extraEnvVarsSecret | string | `""` |  |
| primary.extraPodSpec | object | `{}` |  |
| primary.extraVolumeMounts | list | `[]` |  |
| primary.extraVolumes | list | `[]` |  |
| primary.hostAliases | list | `[]` |  |
| primary.hostIPC | bool | `false` |  |
| primary.hostNetwork | bool | `false` |  |
| primary.initContainers | list | `[]` |  |
| primary.initdb.args | string | `""` |  |
| primary.initdb.password | string | `""` |  |
| primary.initdb.postgresqlWalDir | string | `""` |  |
| primary.initdb.scripts | object | `{}` |  |
| primary.initdb.scriptsConfigMap | string | `""` |  |
| primary.initdb.scriptsSecret | string | `""` |  |
| primary.initdb.user | string | `""` |  |
| primary.labels | object | `{}` |  |
| primary.lifecycleHooks | object | `{}` |  |
| primary.livenessProbe.enabled | bool | `true` |  |
| primary.livenessProbe.failureThreshold | int | `6` |  |
| primary.livenessProbe.initialDelaySeconds | int | `30` |  |
| primary.livenessProbe.periodSeconds | int | `10` |  |
| primary.livenessProbe.successThreshold | int | `1` |  |
| primary.livenessProbe.timeoutSeconds | int | `5` |  |
| primary.name | string | `"primary"` |  |
| primary.nodeAffinityPreset.key | string | `""` |  |
| primary.nodeAffinityPreset.type | string | `""` |  |
| primary.nodeAffinityPreset.values | list | `[]` |  |
| primary.nodeSelector | object | `{}` |  |
| primary.persistence.accessModes[0] | string | `"ReadWriteOnce"` |  |
| primary.persistence.annotations | object | `{}` |  |
| primary.persistence.dataSource | object | `{}` |  |
| primary.persistence.enabled | bool | `true` |  |
| primary.persistence.existingClaim | string | `""` |  |
| primary.persistence.labels | object | `{}` |  |
| primary.persistence.mountPath | string | `"/bitnami/postgresql"` |  |
| primary.persistence.selector | object | `{}` |  |
| primary.persistence.size | string | `"8Gi"` |  |
| primary.persistence.storageClass | string | `""` |  |
| primary.persistence.subPath | string | `""` |  |
| primary.pgHbaConfiguration | string | `""` |  |
| primary.podAffinityPreset | string | `""` |  |
| primary.podAnnotations | object | `{}` |  |
| primary.podAntiAffinityPreset | string | `"soft"` |  |
| primary.podLabels | object | `{}` |  |
| primary.podSecurityContext.enabled | bool | `true` |  |
| primary.podSecurityContext.fsGroup | int | `1001` |  |
| primary.priorityClassName | string | `""` |  |
| primary.readinessProbe.enabled | bool | `true` |  |
| primary.readinessProbe.failureThreshold | int | `6` |  |
| primary.readinessProbe.initialDelaySeconds | int | `5` |  |
| primary.readinessProbe.periodSeconds | int | `10` |  |
| primary.readinessProbe.successThreshold | int | `1` |  |
| primary.readinessProbe.timeoutSeconds | int | `5` |  |
| primary.resources.limits | object | `{}` |  |
| primary.resources.requests.cpu | string | `"250m"` |  |
| primary.resources.requests.memory | string | `"256Mi"` |  |
| primary.schedulerName | string | `""` |  |
| primary.service.annotations | object | `{}` |  |
| primary.service.clusterIP | string | `""` |  |
| primary.service.externalTrafficPolicy | string | `"Cluster"` |  |
| primary.service.extraPorts | list | `[]` |  |
| primary.service.headless.annotations | object | `{}` |  |
| primary.service.loadBalancerIP | string | `""` |  |
| primary.service.loadBalancerSourceRanges | list | `[]` |  |
| primary.service.nodePorts.postgresql | string | `""` |  |
| primary.service.ports.postgresql | int | `5432` |  |
| primary.service.sessionAffinity | string | `"None"` |  |
| primary.service.sessionAffinityConfig | object | `{}` |  |
| primary.service.type | string | `"ClusterIP"` |  |
| primary.sidecars | list | `[]` |  |
| primary.standby.enabled | bool | `false` |  |
| primary.standby.primaryHost | string | `""` |  |
| primary.standby.primaryPort | string | `""` |  |
| primary.startupProbe.enabled | bool | `false` |  |
| primary.startupProbe.failureThreshold | int | `15` |  |
| primary.startupProbe.initialDelaySeconds | int | `30` |  |
| primary.startupProbe.periodSeconds | int | `10` |  |
| primary.startupProbe.successThreshold | int | `1` |  |
| primary.startupProbe.timeoutSeconds | int | `1` |  |
| primary.terminationGracePeriodSeconds | string | `""` |  |
| primary.tolerations | list | `[]` |  |
| primary.topologySpreadConstraints | list | `[]` |  |
| primary.updateStrategy.rollingUpdate | object | `{}` |  |
| primary.updateStrategy.type | string | `"RollingUpdate"` |  |
| psp.create | bool | `false` |  |
| rbac.create | bool | `false` |  |
| rbac.rules | list | `[]` |  |
| readReplicas.affinity | object | `{}` |  |
| readReplicas.annotations | object | `{}` |  |
| readReplicas.args | list | `[]` |  |
| readReplicas.command | list | `[]` |  |
| readReplicas.containerSecurityContext.enabled | bool | `true` |  |
| readReplicas.containerSecurityContext.runAsUser | int | `1001` |  |
| readReplicas.customLivenessProbe | object | `{}` |  |
| readReplicas.customReadinessProbe | object | `{}` |  |
| readReplicas.customStartupProbe | object | `{}` |  |
| readReplicas.extendedConfiguration | string | `""` |  |
| readReplicas.extraEnvVars | list | `[]` |  |
| readReplicas.extraEnvVarsCM | string | `""` |  |
| readReplicas.extraEnvVarsSecret | string | `""` |  |
| readReplicas.extraPodSpec | object | `{}` |  |
| readReplicas.extraVolumeMounts | list | `[]` |  |
| readReplicas.extraVolumes | list | `[]` |  |
| readReplicas.hostAliases | list | `[]` |  |
| readReplicas.hostIPC | bool | `false` |  |
| readReplicas.hostNetwork | bool | `false` |  |
| readReplicas.initContainers | list | `[]` |  |
| readReplicas.labels | object | `{}` |  |
| readReplicas.lifecycleHooks | object | `{}` |  |
| readReplicas.livenessProbe.enabled | bool | `true` |  |
| readReplicas.livenessProbe.failureThreshold | int | `6` |  |
| readReplicas.livenessProbe.initialDelaySeconds | int | `30` |  |
| readReplicas.livenessProbe.periodSeconds | int | `10` |  |
| readReplicas.livenessProbe.successThreshold | int | `1` |  |
| readReplicas.livenessProbe.timeoutSeconds | int | `5` |  |
| readReplicas.name | string | `"read"` |  |
| readReplicas.nodeAffinityPreset.key | string | `""` |  |
| readReplicas.nodeAffinityPreset.type | string | `""` |  |
| readReplicas.nodeAffinityPreset.values | list | `[]` |  |
| readReplicas.nodeSelector | object | `{}` |  |
| readReplicas.persistence.accessModes[0] | string | `"ReadWriteOnce"` |  |
| readReplicas.persistence.annotations | object | `{}` |  |
| readReplicas.persistence.dataSource | object | `{}` |  |
| readReplicas.persistence.enabled | bool | `true` |  |
| readReplicas.persistence.existingClaim | string | `""` |  |
| readReplicas.persistence.labels | object | `{}` |  |
| readReplicas.persistence.mountPath | string | `"/bitnami/postgresql"` |  |
| readReplicas.persistence.selector | object | `{}` |  |
| readReplicas.persistence.size | string | `"8Gi"` |  |
| readReplicas.persistence.storageClass | string | `""` |  |
| readReplicas.persistence.subPath | string | `""` |  |
| readReplicas.podAffinityPreset | string | `""` |  |
| readReplicas.podAnnotations | object | `{}` |  |
| readReplicas.podAntiAffinityPreset | string | `"soft"` |  |
| readReplicas.podLabels | object | `{}` |  |
| readReplicas.podSecurityContext.enabled | bool | `true` |  |
| readReplicas.podSecurityContext.fsGroup | int | `1001` |  |
| readReplicas.priorityClassName | string | `""` |  |
| readReplicas.readinessProbe.enabled | bool | `true` |  |
| readReplicas.readinessProbe.failureThreshold | int | `6` |  |
| readReplicas.readinessProbe.initialDelaySeconds | int | `5` |  |
| readReplicas.readinessProbe.periodSeconds | int | `10` |  |
| readReplicas.readinessProbe.successThreshold | int | `1` |  |
| readReplicas.readinessProbe.timeoutSeconds | int | `5` |  |
| readReplicas.replicaCount | int | `1` |  |
| readReplicas.resources.limits | object | `{}` |  |
| readReplicas.resources.requests.cpu | string | `"250m"` |  |
| readReplicas.resources.requests.memory | string | `"256Mi"` |  |
| readReplicas.schedulerName | string | `""` |  |
| readReplicas.service.annotations | object | `{}` |  |
| readReplicas.service.clusterIP | string | `""` |  |
| readReplicas.service.externalTrafficPolicy | string | `"Cluster"` |  |
| readReplicas.service.extraPorts | list | `[]` |  |
| readReplicas.service.headless.annotations | object | `{}` |  |
| readReplicas.service.loadBalancerIP | string | `""` |  |
| readReplicas.service.loadBalancerSourceRanges | list | `[]` |  |
| readReplicas.service.nodePorts.postgresql | string | `""` |  |
| readReplicas.service.ports.postgresql | int | `5432` |  |
| readReplicas.service.sessionAffinity | string | `"None"` |  |
| readReplicas.service.sessionAffinityConfig | object | `{}` |  |
| readReplicas.service.type | string | `"ClusterIP"` |  |
| readReplicas.sidecars | list | `[]` |  |
| readReplicas.startupProbe.enabled | bool | `false` |  |
| readReplicas.startupProbe.failureThreshold | int | `15` |  |
| readReplicas.startupProbe.initialDelaySeconds | int | `30` |  |
| readReplicas.startupProbe.periodSeconds | int | `10` |  |
| readReplicas.startupProbe.successThreshold | int | `1` |  |
| readReplicas.startupProbe.timeoutSeconds | int | `1` |  |
| readReplicas.terminationGracePeriodSeconds | string | `""` |  |
| readReplicas.tolerations | list | `[]` |  |
| readReplicas.topologySpreadConstraints | list | `[]` |  |
| readReplicas.updateStrategy.rollingUpdate | object | `{}` |  |
| readReplicas.updateStrategy.type | string | `"RollingUpdate"` |  |
| replication.applicationName | string | `"my_application"` |  |
| replication.numSynchronousReplicas | int | `0` |  |
| replication.synchronousCommit | string | `"off"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.automountServiceAccountToken | bool | `true` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `""` |  |
| serviceBindings.enabled | bool | `false` |  |
| shmVolume.enabled | bool | `true` |  |
| shmVolume.sizeLimit | string | `""` |  |
| tls.autoGenerated | bool | `false` |  |
| tls.certCAFilename | string | `""` |  |
| tls.certFilename | string | `""` |  |
| tls.certKeyFilename | string | `""` |  |
| tls.certificatesSecret | string | `""` |  |
| tls.crlFilename | string | `""` |  |
| tls.enabled | bool | `false` |  |
| tls.preferServerCiphers | bool | `true` |  |
| volumePermissions.containerSecurityContext.runAsUser | int | `0` |  |
| volumePermissions.enabled | bool | `false` |  |
| volumePermissions.image.digest | string | `""` |  |
| volumePermissions.image.pullPolicy | string | `"IfNotPresent"` |  |
| volumePermissions.image.pullSecrets | list | `[]` |  |
| volumePermissions.image.registry | string | `"docker.io"` |  |
| volumePermissions.image.repository | string | `"bitnami/bitnami-shell"` |  |
| volumePermissions.image.tag | string | `"11-debian-11-r99"` |  |
| volumePermissions.resources.limits | object | `{}` |  |
| volumePermissions.resources.requests | object | `{}` |  |