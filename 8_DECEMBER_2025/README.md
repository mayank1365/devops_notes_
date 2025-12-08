# Understanding Kubernetes Services

## Overview

Kubernetes Services provide stable networking for pods. Since pods are ephemeral and can be replaced, Services offer a consistent way to access them through a stable IP address and DNS name.

## Key Points

- **ClusterIP**: Default service type, accessible only within cluster
- **NodePort**: Exposes service on each node's IP at a static port
- **LoadBalancer**: Creates external load balancer (cloud provider)
- **ExternalName**: Maps service to external DNS name
- `kubectl expose deployment nginx --port=80 --type=ClusterIP` - Create service
- `kubectl get services` - List all services
- `kubectl describe service service-name` - Get service details
- **Service Discovery**: Pods can find services via DNS
- **Load Balancing**: Distributes traffic across healthy pods
