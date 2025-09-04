# VKS Standard package repo


This example installs an application set that targets all clusters that have a label of `type=vks`. This will install the vks standard repo package so that it can be used to install packages in the cluster.


## Usage

1. connect to the supervisor cluster that argocd is running in and apply the application to the correct namespace.

```bash
kubectl apply -f application.yml -n <supervisor-ns>`
```




