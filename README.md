# k8s
awesome-k8s

This command (with kubectl 1.11+) will show you what resources remain in the namespace:

kubectl api-resources --verbs=list --namespaced -o name \ 
| xargs -n 1 kubectl get --show-kind --ignore-not-found -n <namespace>
  
  
