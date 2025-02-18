# AWS VPC Project

## Project Overview
This project demonstrates the setup of an AWS Virtual Private Cloud (VPC) with multiple subnets, routing configurations, security groups, and a deployed application. The goal is to provide a secure and scalable environment for hosting applications using AWS networking services.

## Architecture
The project follows a structured AWS VPC design, including:
- **VPC** with CIDR block allocation.
- **Public and Private Subnets** for separation of resources.
- **Internet Gateway (IGW)** for external access.
- **NAT Gateway** to allow private subnets to access the internet securely.
- **Route Tables** for proper traffic management.
- **Security Groups** for controlled access to instances.
- **EC2 Instances** deployed in both public and private subnets.

## Components and Services Used
- **AWS VPC**
- **Public and Private Subnets**
- **Internet Gateway (IGW)**
- **NAT Gateway**
- **Route Tables**
- **Security Groups**
- **EC2 Instances**
- **Elastic Load Balancer (Optional)**
- **Auto Scaling (Optional)**

## Deployment Steps
1. **Create a VPC** with a defined CIDR block.
2. **Set up subnets** (public and private).
3. **Attach an Internet Gateway (IGW)** to the VPC for public access.
4. **Create a NAT Gateway** in a public subnet for private subnet internet access.
5. **Define Route Tables** for proper routing between subnets.
6. **Launch EC2 instances** in the respective subnets.
7. **Configure Security Groups** to allow necessary traffic.
8. **Deploy an application** (such as a simple web server) to verify connectivity.

## How to Run
- Clone the repository:
  ```sh
  git clone https://github.com/your-username/aws-vpc-project.git
