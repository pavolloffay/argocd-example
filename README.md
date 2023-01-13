# ArgoCD examples

This repository contains my experiments and examples for ArgoCD.

## Configure the cluster

1. Deploy OpenShift GitOps operator

2. Create a project with ArgoCD configuration

```bash
oc new-project ploffay-argocd-example
oc label namespace ploffay-argocd-example argocd.argoproj.io/managed-by=openshift-gitops
kubectl apply -f application.yaml
```

## Useful commands

```bash
kubectl get applications.argoproj.io
kubectl delete applications.argoproj.io --all
```
