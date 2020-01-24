Regions and availiblity zones (AZs)
- Region (example: eu-west-1, us-east-1, us-east-2). A region has multiple AZs
- An AZ is the logical building block that makes up an AWS Region. Can be made of 1 or more data centers

VPC and SUbnets
- VPC (Virtual private cloud) : logically isolated section of the AWS cloud 
- Subnet: a subset of a VPC. Can be private or public
- subnets can be private or public:
-- public subnets have a default route to an Internet Gateway; private subnets do not.
-- public: 0.0.0.0/0 to igw-xxxxx




TL;DR:
Security group is the firewall of EC2 Instances whereas Network ACL is the firewall of the Subnet.

![VPC Overview](https://miro.medium.com/max/472/1*pwAjuZMHsDJV6XckZGARxA.png)
