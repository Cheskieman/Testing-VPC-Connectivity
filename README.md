# Testing-VPC-Connectivity...... 

## A complete step by step guide to test VPC Connectivity

* Connect to your Public Server from AWS Mamangement Console

* Test connectivity between your EC2 instances
 
* Test VPC connectivity with the internet.

### This project will demostrate how to 

* Set up a VPC & Network ACL

* Create an EC2 Instance and .......


#### Step by Step Instructions guidance

**CREATE VPC & NETWORK ACL**

* Search and Select VPC from AWS Searchbar
<p align="center">  
  <img src="VPCSETUP Select VPC from AWS Searchbar.png alt="Search VPC" width="900" />  
</p>  
* Select Create VPC
<p align="center">  
  <img src="VPCSETUP Select Create VPC intialone.png" alt="Create VPC" width="900" />  
</p>  
* Select VPC and more
<p align="center">  
  <img src="VPCSETUP Select VPC and more.png" alt="Select VPC and more" width="900" />  
</p>  
* Give an specfic name in the auto-generation box.
<p align="center">  
  <img src="VPCSETUP Select VPC and more.png" alt="Select auto generation" width="900" />  
</p>  
* Scroll down and change the availibility zone number to one.
<p align="center">  
  <img src="VPCSETUPCHANGEAVAILIBITYZONEQUANTITY.png" alt="Change Availibility Zone" width="900" />  
</p>  
* Scroll down and click on arrow for Customize subnets CIDR blocks and input the ip addresses displayed in the two subnet boxes.
<p align="center">  
  <img src="VPCSETUPCHANGEAVAILIBITYZONEQUANTITY.png" alt="Select Customizable CIDR" width="900" />  
</p>  
* Scroll down to where it says NAT Gateways and select the option for none.
<p align="center">  
  <img src="VPCSETUP nat gateway select none.png" alt="NAT Gateaway none" width="900" />  
</p>  
* Select Create VPC at bottom.
<p align="center">  
  <img src="VPCSETUP Select CreateVPC bottom.png" alt="Create VPC" width="900" />  
</p>  
* Select Network ACLs from the left hand navigation panel.
<p align="center">  
  <img src="VPCSETUP select network acls from navigation panel.png" alt="Select Network ACL Navigation Panel" width="900" />  
</p>  
* Select the Create network ACL on the top right
<p align="center">  
  <img src="VPCSETUP Click Create Network ACL bootm.png" alt="Create Network ACL" width="900" />  
</p>  
* Give your ACL a name
<p align="center">  
  <img src="VPCSETUP give your acl a name.png" alt="Give Network ACL name" width="900" />  
</p>  
* Select the earlier created VPC
<p align="center">  
  <img src="VPCSETUP Select the earlier created VPC.png" alt="Select earleir created VPC" width="900" />  
</p>  
* Select Create Network ACL at the bottom.
<p align="center">  
  <img src="VPCSETUP Click Create Network ACL bootm.png" alt="Create Network ACL" width="900" />  
</p>  
* Select the Subnet Asscociations tab
<p align="center">  
  <img src="VPCSETUP Select Subnet Asscociations tab.png" alt="Select Subnet Asscociations Tab" width="900" />  
</p>  
* Select Edit Subnet Asscociations
<p align="center">  
  <img src="VPCSETUP Select Edit Subnet Asscociations.png" alt="Select Edit Subnet Asscociations" width="900" />  
</p>  
* Select the private subnet
<p align="center">  
  <img src="VPCSETUP Select Private Subnet.png" alt="Select Private Subnets" width="900" />  
</p>  
* Select Save Changes at bottom.
<p align="center">  
  <img src="VPCSETUP Click save changes at bottom.png" alt="Select Save Changes at bottom" width="900" />  
</p>  
* Select Security Groups from the left hand navigation panel
<p align="center">  
  <img src="VPCSETUP select security groups navigation panel.png" alt="Select Security Group from Left Hand Navigation Panel" width="900" />  
</p>  
* Select Create Security Group on the top right
<p align="center">  
  <img src="VPCSETUP Click Create Security Group at the bottom.png" alt="Select Create Security Group" width="900" />  
</p>  
* Give the Security Group a name.
<p align="center">  
  <img src="VPCSETUP Give securty group a name.png" alt="Give Security Group a Name" width="900" />  
</p>  
* Give a decription for the Security Group
<p align="center">  
  <img src="VPCSETUP give securty group a description.png" alt="Give Description for Security Group" width="900" />  
</p>  
* Select the earlier created VPC
<p align="center">  
  <img src="VPCSETUP Select the earlier created VPC.png" alt="Select Earlier Created VPC" width="900" />  
</p>  
* Select add rule under Inbound rules
<p align="center">  
  <img src="VPCSETUP Select the earlier created VPC.png" alt="Select Add Rules under Inbound Rules" width="900" />  
</p>  
* Select HTTP and anywhere IPV4 as both the type and source for the Inbound Rule
<p align="center">  
  <img src="VPCSETUP set up security group inbound rules.png" alt="Set up Security Inbound Rules" width="900" />  
</p>  
* Select Create Security Group at the bottom.
<p align="center">  
  <img src="VPCSETUP Click Create Security Group at the bottom.png" alt="Select Create Security Group" width="900" />  
</p>  

**Create an EC2 Instance &....**

* Search and Select EC2 from AWS Searchbar

* Select Instances from the left hand navigation panel

* Select Launch Instances from top right

* Give your instance a name

* Select your Keypair

* Select Edit next to Network Settings.










##### Contribution Policy

This project is not accepting external contributions, including pull requests or feature requests.

It serves as a personal archive of my learning journey in applying foundational concepts in software development and version control. Active development is not ongoing, and external changes will not be integrated.

Thank you for your understanding.
