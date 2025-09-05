# Cluster Bootstrap


This example combines a few examples into one. It's purpose is to be a boostrap for clusters. The app set will install an app for  each cluster that it targets and that app will install more apps into the cluster using app sets. so this combines an app set with an app of apps model. For example this could be used to bootstrap all clusters with pakcage repo, obsrvability, ingress, etc.App sets help with the multicluster nature of the supervisor namespace and avoids naming conflicts


## Usage

1. connect to the supervisor cluster that argocd is running in and apply the application to the correct namespace.

```bash
kubectl apply -f application.yml -n <supervisor-ns>`
```




