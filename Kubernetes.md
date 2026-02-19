# Kubernetes cluster commands
- `kubectl cluster-info`                  // Display cluster information
- `kubectl get nodes -o wide`             // List all nodes in the cluster and show IPs

# Kubernetes pod commands
- `kubectl get pods`                      // List all pods
- `kubectl get pods -o wide`              // Show detailed information about a pod
- `kubectl get pods -l <label>=<value>`   // Show pods who have a specific label
- `kubectl get pod <name>`                // Show one specific pod
- `kubectl describe pod <name>`           // Show a pod’s details
- `kubectl logs <pod>`                    // View logs of a pod
- `kubectl exec -it <pod>`                // Execute a command inside a pod
- `kubectl delete pod <pod>`              // Delete a pod
- `kubectl explain pod <resource>`        // Displays an overview of the Pod resource

# Kubernetes deployment commands
- `kubectl create deployment <name> --image=<image>`                   // Create a deployment
- `kubectl get deployments`                                            // List all deployments
- `kubectl describe deployment <name>`                                 // Show deployment details of one deployment
- `kubectl scale deployment <name> --replicas=<number>`                // Increase or decrease deployment
- `kubectl rollout history deployment <name>`                          // Displays the version (revision) history of a deployment.
- `kubectl rollout history deployment <name> --revision=2`             // Detailing a specific review
- `kubectl rollout restart deployment/<name>`                          // Restart a deployment
- `kubectl rollout status deployment/<name>`                           // Show the status of a deployment
- `kubectl create deployment <name> --image=<image> -o yaml`           // Create a deployment and print the YAML
- `kubectl create deployment <name> --image=<image> \` 
  `-o yaml --dry-run=client > name.yaml`                               // Create a deployment without applying it
                                                                       // and store the YAML file inside "name.yaml"

# Kubernetes service commands
- `kubectl get services`                    // List all services
- `kubectl describe service <name>`         // Show service details
- `kubectl expose pod <name>`               // Expose a pod to a service
- `kubectl delete service <name>`           // Delete a service
- `kubectl port-forward <pod> <local-port>:<remote-port>`   // Forward a local port to a pod

# Kubernetes configmap & secret commands
- `kubectl create configmap <name> --from-literal=<key>=<value>`       // Create a ConfigMap
- `kubectl create secret generic <name> --from-literal=<key>=<value>`  // Create a Secret
- `kubectl get configmaps`                                             // List all ConfigMaps
- `kubectl get secrets`                                                // List all Secrets
- `kubectl describe configmap <name>`                                  // Show ConfigMap details

# Kubernetes namespace commands
- `kubectl get namespaces`                                // List all namespaces
- `kubectl create namespace <name>`                       // Create a namespace
- `kubectl delete namespace <name>`                       // Delete namespace
- `kubectl config set-context --current --namespace=<name>`  // Switch to a different namespace

# Kubernetes resource commands
- `kubectl apply -f <file>`                // Apply a resource config file
- `kubectl edit <type> <name>`             // Edit a resource file inside your terminal
- `kubectl delete -f <file>`               // Delete a resource from a config file
- `kubectl get <type>`                     // List resources of a specific type
- `kubectl describe <type> <name>`         // Show details about a specific resource

# Kubernetes statistics & event commands
- `kubectl top nodes`                      // Display node resource usage
- `kubectl top pods`                       // Display pod resource usage
- `kubectl events`                         // Show recent cluster events
- `kubectl get events`                     // List all cluster events

# Kubernetes permissions
- `kubectl get roles`                      // List all roles

