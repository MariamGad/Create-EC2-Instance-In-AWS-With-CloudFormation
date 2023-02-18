# Create-EC2-Instance-In-AWS-With-CloudFormation

## What is CloudFormation
AWS CloudFormation is a service that gives developers and businesses an easy way to create a collection of related AWS and third-party resources, provision and manage them by treating infrastructure as code (IAC).

## Steps of creating an EC2 instance
* Create a new VPC (isolated network) to hold our resources.
* Create a new public-subnet and private-subnet. ***in a VPC we can have one or more subnets***.
* Create Internet Gateway (IGW) to give EC2 instance an access to the Internet.
* Attach The IGW to the VPC.
* Add route table, then route the external traffic to the IGW.
* Associate the route table to our public-subnet.
* Add new security group that allows SSH and HTTP traffic.
* Create a new instance with this security group.
