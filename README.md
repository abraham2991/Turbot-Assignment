# Turbot-Assignment

Login to the AWS account and secure your user
- TO secure user, its best practice to change the password and enable MFA. (I am unable to change the password for this account)



Use Terraform to create a network in AWS’s us-west-2 region:
Delete the default VPC in that region
Create a VPC + 2 Subnets in different availability zones
Create an Internet gateway attached to the VPC
Create a security group that allows ingress from your IP address on port 22 and allows egress to the internet
(0.0.0.0/0) on port 443.
