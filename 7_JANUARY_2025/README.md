# Add an Agent and Implement the CD

## Overview

Continuous Deployment extends CI/CD by automatically deploying every change that passes tests to production. Self-hosted agents provide more control over the deployment environment.

## Key Points

- **Self-Hosted Runners**: Run workflows on your own infrastructure
- **Agent Setup**: Install and configure runner on target server
- `./config.sh --url https://github.com/user/repo --token TOKEN` - Configure agent
- **CD Pipeline**: Automatically deploy after successful CI
- **Deployment Strategies**: Blue-green, canary, rolling updates
- **Environment Variables**: Configure different environments (dev, staging, prod)
- **Health Checks**: Verify deployment success before routing traffic
- **Monitoring**: Track deployments and rollback if needed
- **GitOps**: Use Git as single source of truth for infrastructure
