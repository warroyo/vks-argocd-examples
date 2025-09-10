# VKS observability


This example installs an application set that targets all clusters that have a label of `type=vks`. This will install the vks standard repo package as well as telegraf and prometheus from the package repo. It also configures prometheus and telegraf to use the supervisor management proxy so that metrics are automatically shipped to VCF Ops.


## Usage

1. connect to the supervisor cluster that argocd is running in and apply the application to the correct namespace.

```bash
kubectl apply -f application.yml -n <supervisor-ns>`
```




