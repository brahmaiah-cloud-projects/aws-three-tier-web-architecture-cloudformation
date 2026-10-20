AWS Three-Tier Web Architecture Using CloudFormation
Project Overview
This project deploys a complete Three-Tier Web Architecture on AWS using CloudFormation Nested Stacks.

The solution is highly available and scalable, using an Application Load Balancer, Auto Scaling Group, EC2 instances, and Amazon RDS deployed across multiple Availability Zones.

Architecture
Internet | Application Load Balancer | Target Group | Auto Scaling Group | EC2 Instances | Amazon RDS MySQL

AWS Services Used
Amazon VPC
Public Subnets
Private Application Subnets
Private Database Subnets
Internet Gateway
NAT Gateway
Route Tables
Security Groups
Application Load Balancer
Target Group
Launch Template
Auto Scaling Group
Amazon EC2
Amazon RDS MySQL
AWS CloudFormation
CloudFormation Templates
vpc.yaml
subnet.yaml
igw.yaml
nat.yaml
route-table.yaml
security.yaml
alb.yaml
launch-template.yaml
asg.yaml
rds.yaml
main.yaml
Features
Multi-AZ Deployment
Infrastructure as Code (IaC)
Nested CloudFormation Stacks
Auto Scaling
Load Balancing
Private Database Layer
Highly Available Architecture
Validation
aws cloudformation validate-template \
--template-body file://main.yaml
