Regions and availiblity zones (AZs)
===================================
- Region (example: eu-west-1, us-east-1, us-east-2). A region has multiple AZs
- An AZ is the logical building block that makes up an AWS Region. Can be made of 1 or more data centers

VPC and Subnets
================
- VPC (Virtual private cloud) : logically isolated section of the AWS cloud 
  - can span over multiple AZs
- Subnet: a subset of a VPC. 
  - cannot span multiple AZs
  - an be private or public
    - public subnets have a default route to an Internet Gateway; private subnets do not.
    - public: 0.0.0.0/0 to igw-xxxxx



ACL and Security groups
=======================
TL;DR: Security group is the firewall of EC2 Instances whereas Network ACL is the firewall of the Subnet.
![VPC Overview](https://miro.medium.com/max/472/1*pwAjuZMHsDJV6XckZGARxA.png)

| ACL (Network Access control lists ) | Security Groups |
|-------------------------------------|-----------------|
| applies not subnets and what is in this subnet               | applies to AWS services to which it is explicitely attached to |
| allow everything by default | deny everything by default|
|stateless (need to implement both directions of a communication) | stateful (will allow responses to requests without having explicitely declaring them)|




