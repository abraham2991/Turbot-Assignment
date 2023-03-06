# Turbot-Assignment

# Login to the AWS account and secure your user
------------- To secure user, its best practice to change the password and enable MFA. I was able to enable MFA but I am unable to change the password for this account




# Use Terraform to create a network in AWS’s us-west-2 region:
Delete the default VPC in that region - Terraform adopted the default VPC provisioned by AWS which means Terraform can't handle the deletion of the default VPC
Create a VPC + 2 Subnets in different availability zones, Create an Internet gateway attached to the VPC, Create a security group that allows ingress from your IP address on port 22 and allows egress to the internet (0.0.0.0/0) on port 443. -------------------- All resources were created using Terraform. I made use of Variables too to make the code more reusable, flexible, and maintainable. 






# Fork the turbot/tdk repo
Add a top level folder named customer_success_test
In that folder create a python script list_user_policies.py
That script should iterate over all users in the account, listing the iam policies attached to each user.
Create a pull request for your fork.  ----------------------- All done, please see branch abraham/ft https://github.com/abraham2991/tdk.git 






# Create a compute resource:
Deploy a linux based t3.micro EC2 instance into the VPC created above ----------------- Resource was created using Terraform
Clone the forked repo to the instance, run your python code -------------------------- Git was installed on the instance, repo cloned, a python virtual environment was initiated(venv) to run the python code that was pulled from the repo. After successful run, the IAM policies attached to the users was displayed.
Stop the EC2 instance --------------------- EC2 was stopped.
