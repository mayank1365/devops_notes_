# Introduction to Infrastructure Provisioning and Terraform

## Overview

Terraform is an Infrastructure as Code (IaC) tool that allows you to define and provision infrastructure using declarative configuration files. It supports multiple cloud providers and on-premises solutions.

## Key Points

- **Infrastructure as Code**: Define infrastructure in version-controlled files
- **Declarative Syntax**: Describe desired state, Terraform handles how to achieve it
- **Provider**: Plugin that interacts with cloud platforms (AWS, Azure, GCP)
- **Resource**: Infrastructure component (VM, network, database)
- **State File**: Tracks current infrastructure state
- `terraform init` - Initialize working directory
- `terraform plan` - Preview changes before applying
- `terraform apply` - Create/update infrastructure
- `terraform destroy` - Remove all managed infrastructure
- **Modules**: Reusable infrastructure components
