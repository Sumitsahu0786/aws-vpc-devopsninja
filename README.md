# aws-vpc-devopsninja
AWS VPC Networking Project with Public and Private Subnets
# AWS VPC Networking Project – devopsninja

## Project Overview
This project demonstrates the creation and configuration of a custom Amazon Virtual Private Cloud (VPC) using AWS.

The VPC contains two public subnets and two private subnets with separate route tables.

## AWS Services Used
- Amazon VPC
- Public and Private Subnets
- Internet Gateway (IGW)
- Route Tables
- Availability Zones

## VPC Configuration

| Configuration | Value |
|---|---|
| VPC Name | devopsninja |
| VPC CIDR | 192.168.0.0/16 |

## Subnet Configuration

### Public Subnets

| Subnet | CIDR |
|---|---|
| Public Subnet 1 | 192.168.0.0/19 |
| Public Subnet 2 | 192.168.32.0/19 |

### Private Subnets

| Subnet | CIDR |
|---|---|
| Private Subnet 1 | 192.168.64.0/19 |
| Private Subnet 2 | 192.168.96.0/19 |

## Internet Gateway
Created and attached an Internet Gateway named `devopsninja-igw` to the VPC.

## Routing Configuration

### Public Route Table
- 192.168.0.0/16 → local
- 0.0.0.0/0 → Internet Gateway

Associated with both public subnets.

### Private Route Table
- 192.168.0.0/16 → local

Associated with both private subnets.

## Architecture Diagram

![AWS VPC Architecture](architecture/aws-vpc-architecture.png)

## Key Learnings
- Understanding AWS VPC networking.
- Creating public and private subnets.
- Configuring Internet Gateway.
- Creating and associating route tables.
- Understanding public and private network routing.

## Project Status
Completed: VPC, subnets, Internet Gateway, and route table configuration.

## Future Improvements
- Deploy EC2 instances.
- Configure NAT Gateway.
- Implement a 3-tier architecture.
- Automate infrastructure using Terraform.

## Author
Cloud & DevOps 

**Learning by Doing | AWS Cloud | DevOps**
