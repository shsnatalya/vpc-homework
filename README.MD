HOW TO CREATE VPC?
1. Type VPC in search in your AWS account and identify the region needed.
In 1 region we can have maximum 5 VPCs.
2. We mark VPC only (VPC and more is used for companies).
3. Provide the name for VPC.
4. In IPV4 CIDR we should provide the subnet mask (depends on how many IP addresses we need). You must specify IP address ranges for your VPC and subnets. For more information, see IP addressing for your VPCs and subnets.
5. Tenancy - special option for VPC, should always be default. 
6. Add tags.
7. Create VPC.
8. We’re creating subnet(s) for VPC.
9. Creating a subnet we’re choosing our VPC.
10. Create a name for subnet (Public and Private)
11. WE choose availability zone in which subnet will reside.
12. IPV4 subnet CIDR block - we specify amount of IP adreses (e.g. 10.0.1.0/24). 
13. Create subnet. Repeat same procedure for private one. A range of IP addresses in your VPC. You can launch AWS resources, such as EC2 instances, into your subnets. Each subnet resides entirely within one Availability Zone. By launching instances in at least two Availability Zones, you can protect your applications from the failure of a single Availability Zone. 
15. For Public subnet we have to be connected to the Internet. 
16. Click on Internet Gateway - create Internet Gateway. Connects your VPC to the internet. The instances in a public subnet can access the internet because the subnet route table contains a route that sends traffic bound for the internet to the internet gateway. 
17. Create a name for Internet Gateway.
18. Create tags and create a gateway. 
19. By default all subnets are private. Once we attach Internet Gateway to subnet -  it becomes public. We have to create a route for that. We have to create an Internet Gateway and attach it to VPC to connect it to Internet.
20. We need to provide a path from Public Subnet to Internet Gateway using route table.
21. Create route table - specify public
22. Select VPC
23. Add tags.
24. Create route table. Contains a set of rules, called routes, that determine where network traffic from your subnet or gateway is directed.
25. Do same for private subnet- create private route table.
26. Go back to route tables.
27. Click on subnet association - we have to choose our public subnets - we specify range we give to those IP dresses and save associations. 
28. Create a route for internet gateway - click on routes - edit routes.
29. Add toute - change destination - specify the range of IP addresses and choose destination from the list (e.g. Internet Gateway/Instance/etc).
30. Create NAT Gateway - give the name. Enables instances in a private subnet to send outbound traffic to the internet, but prevents resources on the internet from connecting to the instances. In production, we recommend that you deploy a NAT gateway in each active AZ. 
31. Choose the subnet (always should be public).
32. Connectivity type - should always be public.
33. Assign an elastic IP dress by clicking n allot Elastic IP.
34. Create tags and create.



