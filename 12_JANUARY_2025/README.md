# Terraform in Action

## Overview

Practical Terraform usage involves writing configuration files, managing state, and organizing infrastructure code. Best practices include using modules, remote state, and proper variable management.

## Key Points

- ```hcl
resource "aws_instance" "web" {
  ami           = "ami-0c55b159cbfafe1f0"
  instance_type = "t2.micro"
  tags = {
    Name = "WebServer"
  }
}
```
- **Variables**: `variable "region" { default = "us-east-1" }`
- **Outputs**: `output "instance_ip" { value = aws_instance.web.public_ip }`
- **Remote State**: Store state in S3 or Terraform Cloud
- **Workspaces**: Manage multiple environments with same configuration
- **Data Sources**: Query existing infrastructure
- `terraform fmt` - Format configuration files
- `terraform validate` - Check configuration syntax
- **Import**: Bring existing infrastructure under Terraform management
