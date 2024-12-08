# Virtual_networking
# VPC
<BR>
A virtual private cloud (VPC) is a virtual network dedicated to your AWS account. It is logically isolated from 
other virtual networks in the AWS Cloud. You can launch your AWS resources, such as Amazon EC2 instances, into your 
VPC.

![image](https://github.com/user-attachments/assets/68942c35-be00-4be2-8234-d282f5941caf)
**AWS Console -> Services -> Networking & Content Delivery -> VPC -> Your VPCs**
<BR><BR>
**VPC Name: MyVPC**
<BR><BR>
**IPv4 CIDR Block: 10.0.0.0/16**
<BR><BR>
**Click Create**
<BR><BR>
![image](https://github.com/user-attachments/assets/da5059b1-86d6-435d-bf30-33d41c763722)

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
![image](https://github.com/user-attachments/assets/ab5031b4-68fb-45e6-a398-ce8510708bd8)

**Create Internet gateway**
<BR><BR>
**Now attach Internet Gateway to VPC**
<BR><BR>
**Create Virtual Private Gateway**
<BR><BR>
**Now attach Virtual Private Gateway to VPC**
<BR><BR>
**Create route tables and attach to subnets**
![image](https://github.com/user-attachments/assets/398c7e75-bf74-41fe-9aff-79c3d16e1db0)

# ELB
**Launch two EC2 instances in different AZs**
<BR><BR>
![image](https://github.com/user-attachments/assets/d31539f4-de35-48f9-8b3d-e92983bae6d5)

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
![393568206-cea97452-ac1c-4cf4-ac58-ecff83fc58a3 (1)](https://github.com/user-attachments/assets/6fc3c96a-f45b-4819-996d-8d803fb7aea2)

