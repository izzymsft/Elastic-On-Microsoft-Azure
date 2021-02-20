
## Deploying Elastic on Azure Kubernetes Service

```bash

# Deploy the first Helm Chart to install the Operator
helm upgrade --install elastic-foundation Elastic-Foundation

# Deploy the second Helm Chart to install your resources
helm upgrade --install elastic-resources Elastic-Resources

# Run this command to checkout the pods
kubectl get pods

# Run these commands look for the public ips/port numbers for the services
kubectl get svc


```
