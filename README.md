# AWS VPC Project: Secure Application Deployment in Private Subnet

This project demonstrates the implementation of a secure AWS Virtual Private Cloud (VPC) with public and private subnets, NAT Gateway, Internet Gateway, Auto Scaling Groups, and Application Load Balancer. The goal is to deploy a Python application in a private subnet while ensuring secure access and scalability.

## **Project Overview**

- **VPC**: Created a VPC with the IP range `172.16.0.0/16`.
- **Subnets**: Divided the VPC into public and private subnets across two availability zones for high availability.
- **Internet Gateway (IGW)**: Attached to the VPC to allow internet access for resources in the public subnet.
- **NAT Gateway**: Configured to allow instances in the private subnet to access the internet securely without exposing their private IP addresses.
- **Auto Scaling Group**: Deployed EC2 instances in the private subnet to ensure scalability and high availability.
- **Application Load Balancer (ALB)**: Configured in the public subnet to distribute traffic to the EC2 instances in the private subnet.
- **Bastion Host**: Used to securely access EC2 instances in the private subnet via SSH.

## **Architecture Diagram**

<img width="280" alt="image" src="https://github.com/user-attachments/assets/02c93bd9-eb4a-42bf-b94f-1a3e6bb61838" />


## **Steps to Implement the Project**

1. **Create a VPC**: Defined an IP address range and created public and private subnets in two availability zones.
2. **Set Up Internet Gateway (IGW)**: Attached an IGW to the VPC for internet access.
3. **Configure NAT Gateway**: Set up a NAT Gateway in the public subnet to allow private subnet instances to access the internet securely.
4. **Launch EC2 Instances**: Used an Auto Scaling Group to deploy EC2 instances in the private subnet.
5. **Set Up Bastion Host**: Created a Bastion Host in the public subnet to securely access EC2 instances in the private subnet.
6. **Deploy Application**: Installed a Python application on one of the EC2 instances in the private subnet.
7. **Configure Application Load Balancer (ALB)**: Set up an ALB in the public subnet to distribute traffic to the EC2 instances.
8. **Test Connectivity**: Verified that the application is accessible via the ALB and that instances in the private subnet can access the internet via the NAT Gateway.

## **Tools and Technologies Used**

- **AWS Services**: VPC, EC2, IGW, NAT Gateway, Auto Scaling Groups, Application Load Balancer, Security Groups.
- **Networking Concepts**: Subnetting, Routing, NAT, Load Balancing.
- **Cloud Concepts**: High Availability, Scalability, Security.

## **Learning Outcomes**

- Gained hands-on experience with AWS VPC and its components.
- Learned how to securely deploy applications in private subnets.
- Understood how to configure Auto Scaling Groups and Load Balancers for scalability and high availability.
- Developed a strong foundation in cloud networking and security.

## **References**

- [AWS VPC Documentation](https://docs.aws.amazon.com/vpc/)
- [YouTube Tutorial](https://www.youtube.com/watch?v=P8g7Z4NYk3Q)
