Auto Scaling Group with ELB example
Configuration in this directory creates Launch Configuration, Auto Scaling Group, Elastic Load Balancer and places Auto Scaling EC2 instances under ELB.

Data sources are used to discover existing VPC resources (VPC, subnet and security group) as well as AMI details.

Usage
To run this example you need to execute:

$ terraform init
$ terraform plan
$ terraform apply
Note that this example may create resources which cost money. Run terraform destroy when you don't need these resources.

Outputs
Name	Description
this_autoscaling_group_id	   The autoscaling group id
this_elb_dns_name	           DNS Name of the ELB
this_launch_configuration_id	   The ID of the launch configuration