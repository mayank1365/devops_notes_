# Deep Dive into Kubernetes ReplicaSets

## Overview

ReplicaSets ensure that a specified number of pod replicas are running at any given time. They provide high availability and load distribution by maintaining a stable set of replica pods.

## Key Points

- `kubectl get replicasets` - List all ReplicaSets
- `kubectl describe rs replicaset-name` - Get ReplicaSet details
- `kubectl scale rs replicaset-name --replicas=5` - Scale ReplicaSet
- **Selector**: Labels used to identify which pods belong to the ReplicaSet
- **Replicas**: Desired number of pod copies to maintain
- **Template**: Pod template used to create new pods
- **Self-Healing**: Automatically replaces failed pods
- **Label Matching**: Uses label selectors to manage pods
- **Not Recommended Directly**: Usually managed by Deployments
