# Platform Services

Helm Charts und Konfigurationen fuer zentrale Plattform-Services auf Kubernetes.

## Services

| Service | Version | App Version | Beschreibung |
|---------|---------|-------------|--------------|
| [Alerta](alerta/) | 0.4.0 | 8.7.0 | Monitoring und Alerting |
| [Keycloak](keycloak/) | 7.1.11 | 26.5.6 | Identity and Access Management (SSO, OAuth, SAML, LDAP) |
| [Vault](vault/) | 0.32.0 | 1.21.2 | Secrets Management und Encryption |

## Struktur

Jeder Service-Ordner enthaelt:

- `Chart.yaml` - Helm Chart Definition
- `values.yaml` - Konfigurationswerte

## Verwendung

```bash
# Chart installieren (Beispiel: Vault)
helm install vault ./vault -f vault/values.yaml
```
