# Secret Store Integration


This example installs an application set that targets all clusters that have a label of `type=vks`. This will install the vault agent injector into the cluster so that it can be used with teh secret store service. 


## Usage

1. edit the application.yml and replace the address of the secret store server
2. connect to the supervisor cluster that argocd is running in and apply the application to the correct namespace.


```bash
kubectl apply -f application.yml -n <supervisor-ns>`
```




