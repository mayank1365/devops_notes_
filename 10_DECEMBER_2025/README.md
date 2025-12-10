# Deep Dive into Kubernetes Services

## Overview

Advanced service concepts include endpoint management, session affinity, and headless services. Understanding these patterns is crucial for building robust microservices architectures.

## Key Points

- **Endpoints**: Backend pods that service routes traffic to
- `kubectl get endpoints service-name` - View service endpoints
- **Session Affinity**: Route requests from same client to same pod
- **Headless Services**: ClusterIP set to None, returns pod IPs directly
- **Service Mesh**: Advanced traffic management with tools like Istio
- **Port Naming**: Name ports in pod spec for better service configuration
- `targetPort` - Port on the pod to forward traffic to
- `port` - Port exposed by the service
- `nodePort` - Port exposed on each node (30000-32767 range)
