# K8-s


🔧 Kubernetes Commands for DevOps Engineers 🚀

Here’s a handy list of essential Kubernetes commands to streamline your workflow and boost your productivity. Save this post for quick reference! 📌


🔹 Cluster Management:

# Check cluster info
kubectl cluster-info

# Get all nodes
kubectl get nodes

# Describe a node
kubectl describe node <node-name>

# Check cluster health
kubectl get componentstatuses

🔹 Namespaces:

# List all namespaces
kubectl get namespaces

# Create a namespace
kubectl create namespace <namespace-name>

# Delete a namespace
kubectl delete namespace <namespace-name>

🔹 Pods:

# List all pods in the default namespace
kubectl get pods

# List pods in a specific namespace
kubectl get pods -n <namespace>

# Describe a pod
kubectl describe pod <pod-name>

# Delete a pod
kubectl delete pod <pod-name>

🔹 Deployments:

# List all deployments
kubectl get deployments

# Create a deployment
kubectl create deployment <deployment-name> --image=<image-name>

# Update a deployment
kubectl set image deployment/<deployment-name> <container-name>=<new-image>

# Scale a deployment
kubectl scale deployment <deployment-name> --replicas=<number>

# Delete a deployment
kubectl delete deployment <deployment-name>

🔹 Services:

# List all services
kubectl get services

# Create a service
kubectl expose deployment <deployment-name> --type=<type> --port=<port>

# Describe a service
kubectl describe service <service-name>

# Delete a service
kubectl delete service <service-name>

🔹 ConfigMaps & Secrets:

# List all ConfigMaps
kubectl get configmaps

# Create a ConfigMap
kubectl create configmap <configmap-name> --from-literal=<key>=<value>

# List all Secrets
kubectl get secrets

# Create a Secret
kubectl create secret generic <secret-name> --from-literal=<key>=<value>

🔹 Persistent Volumes & Claims:

# List all persistent volumes
kubectl get pv

# List all persistent volume claims
kubectl get pvc

# Create a persistent volume
kubectl apply -f <persistent-volume-definition>.yaml

# Create a persistent volume claim
kubectl apply -f <persistent-volume-claim-definition>.yaml

🔹 Logs & Monitoring:

# View logs of a pod
kubectl logs <pod-name>

# View logs of a specific container in a pod
kubectl logs <pod-name> -c <container-name>

# Stream logs of a pod
kubectl logs -f <pod-name>

🔹 Troubleshooting:

# Get events
kubectl get events

# Describe a resource
kubectl describe <resource-type> <resource-name>

# Exec into a pod
kubectl exec -it <pod-name> -- /bin/bash

🔹 Custom Resources:

# List custom resource definitions
kubectl get crd

# Describe a custom resource
kubectl describe crd <custom-resource-name>
