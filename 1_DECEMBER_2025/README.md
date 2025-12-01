# Deep Dive into Kubernetes Pods

## Overview

Pods are the fundamental building blocks in Kubernetes. A Pod represents a single instance of a running process in your cluster and can contain one or more tightly coupled containers that share resources.

## Key Points

- `kubectl run nginx --image=nginx` - Create a simple pod
- `kubectl get pods` - List all pods
- `kubectl describe pod pod-name` - Get detailed pod information
- `kubectl logs pod-name` - View pod logs
- `kubectl exec -it pod-name -- bash` - Execute commands in pod
- `kubectl delete pod pod-name` - Delete a pod
- **Shared Network**: Containers in a pod share the same IP address
- **Shared Storage**: Pods can share volumes between containers
- **Pod Lifecycle**: Pending → Running → Succeeded/Failed
- **Init Containers**: Run before app containers to perform setup tasks
