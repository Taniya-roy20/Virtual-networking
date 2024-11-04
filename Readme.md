# Virtual_networking
# VPC
<BR><BR>
**AWS Console -> Services -> Networking & Content Delivery -> VPC -> Your VPCs**
<BR><BR>
**VPC Name: MyVPC**
<BR><BR>
**IPv4 CIDR Block: 10.0.0.0/16**
<BR><BR>
**Click Create**
<BR><BR>
# Create subnets :-
<BR><BR>
**S1-Private Us-east-2a 10.0.1.0/24 Private**
<BR><BR>
**S2-Private Us-east-2b 10.0.2.0/24 Private**
<BR><BR>
**S3-Public Us-east-2a 10.0.3.0/24 Public**
<BR><BR>
**S4-Public Us-east-2b 10.0.4.0/24 Public**
<BR><BR>
**Create Internet gateway**
<BR><BR>
**Now attach Internet Gateway to VPC**
<BR><BR>
**Create Virtual Private Gateway**
<BR><BR>
**Now attach Virtual Private Gateway to VPC**
<BR><BR>
**Create route tables and attach to subnets**
# ELB
**Launch two EC2 instances in different AZs**
<BR><BR>
**Select Application Elastic Load Balancer**
<BR><BR>
**Create 2 instances of same type with select VPC which you created and using putty download apache-2 on both**
<BR><BR>
**Create Target group and attach both ec2 instances we created and edit health check-ups as:-**
<BR><BR>
**Now select this target group and create load balancer**
<BR><BR>
**Now copy your load balancers dns name and paste it in another tab and refersh twice to see it working**
<BR><BR>
**On any one instance write following commands in putty**

       seq 999999999999999999999 > /dev/null &
       
       htop
