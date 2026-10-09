# AWS VPC Terraform Basics

An introductory Terraform lab that provisions a single AWS VPC in `ap-southeast-2` (Sydney). It was built to learn the Terraform workflow on AWS (provider configuration, init, plan, apply, destroy) alongside existing Azure experience.

## What it deploys

| Resource | Details |
|---|---|
| VPC | `10.0.0.0/16`, tagged `vpc-terraform-lab` |

## Usage

Requires Terraform and AWS credentials configured locally (for example through `aws configure` using a least privilege IAM user).

```
terraform init
terraform plan
terraform apply
terraform destroy
```

## Scope

This repository covers the basics only. It does not yet include subnets, an internet gateway, route tables or security groups.

## Next steps

- Add public and private subnets across two Availability Zones.
- Add an internet gateway and route tables.
- Add security groups and a test EC2 instance.
