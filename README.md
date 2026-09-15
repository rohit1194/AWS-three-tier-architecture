# Highly Available 3-Tier AWS Architecture

## Overview

This project demonstrates a highly available and secure 3-tier architecture on AWS using a custom VPC, public and private subnets, Application Load Balancer, Auto Scaling EC2 instances, and Amazon RDS MySQL.

The architecture is designed to keep the application and database layers private while exposing only the load balancer to the internet.

---

## Architecture

```text
Internet
   |
   v
Internet Gateway
   |
   v
Application Load Balancer
Public Subnets
   |
   v
Target Group
   |
   v
Auto Scaling Group
Private Application Subnets
   |
   v
EC2 Instances + Nginx
   |
   v
RDS MySQL
Private Database Subnets
