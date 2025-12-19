# A Simple CI Using GitHub Actions

## Overview

GitHub Actions is a CI/CD platform integrated into GitHub. It allows you to automate workflows directly from your repository using YAML configuration files.

## Key Points

- **Workflow File**: `.github/workflows/ci.yml` defines automation
- **Triggers**: `on: [push, pull_request]` specifies when to run
- **Jobs**: Independent tasks that run in parallel or sequence
- **Steps**: Individual commands within a job
- **Runners**: Virtual machines that execute workflows
- **Actions**: Reusable units of code from marketplace
- ```yaml
name: CI
on: [push]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Run tests
        run: npm test
```
- **Secrets**: Store sensitive data like API keys securely
- **Matrix Builds**: Test across multiple versions/platforms
