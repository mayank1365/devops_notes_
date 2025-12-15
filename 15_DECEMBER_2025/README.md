# Understanding HPA (Horizontal Pod Autoscaler)

## Overview

Horizontal Pod Autoscaler automatically scales the number of pods based on observed CPU utilization, memory usage, or custom metrics. It ensures applications can handle varying loads efficiently.

## Key Points

- `kubectl autoscale deployment nginx --cpu-percent=50 --min=1 --max=10` - Create HPA
- `kubectl get hpa` - List horizontal pod autoscalers
- `kubectl describe hpa hpa-name` - Get HPA details
- **Metrics Server**: Required for HPA to collect resource metrics
- **Scale Up**: Adds pods when metrics exceed threshold
- **Scale Down**: Removes pods when metrics drop below threshold
- **Cooldown Period**: Prevents rapid scaling fluctuations
- **Custom Metrics**: Scale based on application-specific metrics
- **Resource Requests**: Pods must have CPU/memory requests defined
