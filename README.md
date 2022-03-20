# cs4843assignment2

#Website link: http://assign2-albn-539650302.us-east-1.elb.amazonaws.com/

Create a VPC in a selected region with your specific IP i.e 172.20.0.0

Create 9 subnets for the VPC with first 3 public, next the private ones and then last 3 for the databases.

Create routing tables for the subnets and associations for each. Additionally make one(the first one for me) be the internet gateway. Have NAT gateways for the private subnets and the database subnets and finish the associations for each one.

Launch a EC2 instance with the VPC being the one created before and the subnet will be the internet gateway one. Create a security group for this instance with whatever details desired. Have a keypair for this instance and download it.
Create 2 more instances for the application subnets and an additional security group specifically for these two instances. Run through the first EC2 instance because that is the internet gateway. Have the same keypair or a different one for these app servers if desired.

Install necessary php/apache services within the application instance to get the webpage up and running. Taken from https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-lamp-amazon-linux-2.html.

Configure an application load balancer with targeting on the application instances. Create a new security group for the load balancer with whatever settings needed.
Website is now up and running with the basics
