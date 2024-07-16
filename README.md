# infrastructure-using-terraform
Setting up an infrastructure in AWS using Terraform(HCL)

#Project Overview
This project involves creating a highly available and scalable web application infrastructure using Terraform to manage AWS resources. The setup includes a Virtual Private Cloud (VPC), two public subnets, an Internet Gateway, an Application Load Balancer (ALB), EC2 instances in different Availability Zones (AZs), and an Amazon S3 bucket for data storage. The objective is to ensure high availability and efficient load distribution across the instances.

Step-by-Step Implementation using Terraform

Creating the VPC:
- Define a VPC with a specified CIDR block.
- Ensure that the VPC serves as the network boundary for your application.

Setting Up Public Subnets:
- Create two public subnets within the VPC, each in a different Availability Zone.
- These public subnets will allow resources within them to communicate directly with the internet.
- Deploying Applications in Different Availability Zones:

Launch EC2 instances in each of the public subnets using Terraform.
- Ensure that the instances are in separate Availability Zones to maintain high availability.
- Configuring the Internet Gateway:

Attach an Internet Gateway to the VPC using Terraform.
- The Internet Gateway will enable internet access to the resources within the VPC.

Setting Up the Load Balancer:
- Create an Application Load Balancer (ALB) using Terraform to distribute incoming traffic across the EC2 instances.
- The ALB ensures efficient load balancing and improves the fault tolerance of your applications.

Using Amazon S3 for Data Storage:
- Set up an Amazon S3 bucket to store data that will be used by both applications.
- S3 provides a highly available and durable storage solution that can be accessed from your EC2 instances.

Conclusion
- By using Terraform, you can automate the provisioning of a robust, highly available, and scalable architecture for your web applications. This Terraform configuration file sets up a VPC, public subnets, Internet Gateway, Application Load Balancer, EC2 instances, and an S3 bucket, ensuring that your applications are accessible, resilient, and can handle varying loads efficiently.
