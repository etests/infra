# infra

## Create an ArgoCD Application

To create an ArgoCD application, use the following command:

```sh
argocd app create etests-django \
  --repo https://github.com/etests/infra.git \
  --path charts/etests-django \
  --dest-server https://kubernetes.default.svc \
  --dest-namespace default
```
