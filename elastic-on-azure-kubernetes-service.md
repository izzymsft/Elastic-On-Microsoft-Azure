
## Deploying Elastic on Azure Kubernetes Service

Navigate to the directory containing the Helm Charts

Install the first Helm Chart to set up the foundational resources

Then, install the second Helm chart to install the resources for your cluster

Once the resources are installed, you can check out the resources that have been deployed

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
