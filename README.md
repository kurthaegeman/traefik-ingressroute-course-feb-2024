# Traefik IngressRoute training Feb 15

This repo contains the YAML files used in my February 15th training session on
using Traefik IngressRoute on Kubernetes to expose your HTTP-based
applications.

## Test your apps

Create an `/etc/hosts` file with the `Host` entries you picked in the
IngressRoute.

## Useful links

- [Traefik and Kubernetes](https://doc.traefik.io/traefik/routing/providers/kubernetes-crd/)
- [overview of the available Traefik middlewares](https://doc.traefik.io/traefik/middlewares/overview/)
- [rate-limiting example](https://traefik.io/blog/kubernetes-crds-in-traefik/)
- routing TCP
  - [IngressRouteTCP](https://doc.traefik.io/traefik/routing/providers/kubernetes-crd/#kind-ingressroutetcp)
  - [Traefik TCP router](https://doc.traefik.io/traefik/routing/routers/#configuring-tcp-routers)
