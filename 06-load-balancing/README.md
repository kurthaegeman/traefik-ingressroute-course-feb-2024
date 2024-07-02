# Load balancing / canary deployments

[TraefikService](https://doc.traefik.io/traefik/routing/providers/kubernetes-crd/#kind-traefikservice)
allows you to use any (valid) combinations of:

- Weighted Round Robin load balancing
- Mirroring

Allows for [rolling deployments and canary
deployments](https://traefik.io/glossary/kubernetes-deployment-strategies-blue-green-canary/).

For this example, we are deploying everything in the same namespace.

```bash
while true; do http --body https://product.nomadrail.com/meta; sleep 1; done
{
    "release": "the original version",
    "version": "v1.0"
}


{
    "release": "the new version",
    "version": "v2.0"
}


{
    "release": "the original version",
    "version": "v1.0"
}
```
