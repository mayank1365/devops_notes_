# Deep Dive into Kubernetes Deployments

## Overview

Deployments provide declarative updates for Pods and ReplicaSets. They enable rolling updates, rollbacks, and scaling while maintaining application availability during updates.

## Key Points

- `kubectl create deployment nginx --image=nginx:1.21` - Create deployment
- `kubectl get deployments` - List deployments
- `kubectl scale deployment nginx --replicas=3` - Scale deployment
- `kubectl set image deployment/nginx nginx=nginx:1.22` - Update image
- `kubectl rollout status deployment/nginx` - Check rollout status
- `kubectl rollout undo deployment/nginx` - Rollback to previous version
- `kubectl rollout history deployment/nginx` - View rollout history
- **Rolling Updates**: Gradually replace old pods with new ones
- **Zero Downtime**: Maintains availability during updates
- **Revision History**: Keep track of deployment changes
