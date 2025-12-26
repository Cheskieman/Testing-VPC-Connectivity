# Testing-VPC-Connectivity...... 

## A complete step by step guide to test VPC Connectivity

* Connect to your Public Server from AWS Mamangement Console

* Test connectivity between your EC2 instances
 
* Test VPC connectivity with the internet.

### This project will demonstrate how to 

* Set up a VPC & Network ACL

* Create two seperate EC2 Instances

* Connect to the EC2 instance using EC2 Instance Connect after resolving the connection error

* Test connectivity between both EC2 Instances that were created


#### Step by Step Instructions guidance

**CREATE VPC & NETWORK ACL**

* Search and Select VPC from AWS Searchbar
<p align="center">  
  <img src="VPCSETUP Select VPC from AWS Searchbar.png" alt="Search VPC" width="900" />  
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
  <img src="VPCSETUP Auto Generation Give Name.png" alt="Give name auto generation box" width="900" />  
</p>  
* Scroll down and change the availibility zone number to one.
<p align="center">  
  <img src="VPCSETUPCHANGEAVAILIBITYZONEQUANTITY.png" alt="Change Availibility Zone" width="900" />  
</p>  
* Scroll down and click on arrow for Customize subnets CIDR blocks and input the ip addresses displayed in the two subnet boxes.
<p align="center">  
  <img src="VPCSETUP Change the customize suubnets CIDR blocks.png" alt="Select Customizable CIDR" width="900" />  
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
* Select the recently created ACL
  <p align="center">  
  <img src="Nextwork Private NACL select.png" alt="Select recently created ACL" width="900" />  
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
  <img src="VPCSETUP add rule inbound security group.png" alt="Select Add Rules under Inbound Rules" width="900" />  
</p>  
* Select HTTP and anywhere IPV4 as both the type and source for the Inbound Rule
<p align="center">  
  <img src="VPCSETUP set up security group inbound rules.png" alt="Set up Security Inbound Rules" width="900" />  
</p>  
* Select Create Security Group at the bottom.
<p align="center">  
  <img src="VPCSETUP Click Create Security Group at the bottom.png" alt="Select Create Security Group" width="900" />  
</p>  

**Create an EC2 Instance & Attach Appropiate Security Groups**

* Search and Select EC2 from AWS Searchbar
<p align="center">  
  <img src="EC2 Select EC2 from searchbar.png" alt="Select EC2 AWS Searchbar" width="900" />  
</p>  
* Select Instances from the left hand navigation panel
<p align="center">  
  <img src="EC2 Select Instances from Navigation Panel.png" alt="Select Instances from Navigation Panel" width="900" />  
</p>  
* Select Launch Instances from top right
<p align="center">  
  <img src="EC2 Select Launch Instances from top right.png" alt="Select Launch Instance" width="900" />  
</p>  
* Give your instance a name(that represents that this is a Public Server).
<p align="center"> 
  <img src="EC2 give instance a name.png" alt="Give Instance Name" width="900" />  
</p>  
* Select your Keypair
<p align="center">  
  <img src="EC2 Select Keypair.png" alt="Select Keypair" width="900" />  
</p>  
* Select Edit next to Network Settings.
<p align="center">  
  <img src="EC2 Select edit instance network settings.png" alt="Select Edit" width="900" />  
</p>  
* Select the VPC created from earleir
<p align="center">  
  <img src="VPCSETUP Select the vpc created earlier for security group setup.png" alt="Select Earlier Created VPC" width="900" />  
</p>  
* Select the Public Subnet created from earlier
<p align="center">  
  <img src="EC2 Select Instance Network Settings Public Subnet that I set up earlier.png" alt="Select Public Subnet Earlier" width="900" />  
</p>  
* Select Enable for Auto-assign public IP
<p align="center">  
  <img src="EC2 instance network settings enable auto-assign public ip.png" alt="Select Enable " width="900" />  
</p>  
* Select existing security group
<p align="center">  
  <img src="EC2 network settings firewall select existing security group.png" alt="Select Existing Security Group" width="900" />  
</p>  
* Select the Security group created from earlier
<p align="center">  
  <img src="EC2 Instance Network Setting Select Security Group Created earlier.png" alt="Select earlier created Security Group" width="900" />  
</p>  
* Select Launch Instance at the bottom
<p align="center">  
  <img src="EC2 Instance Select Launch Instance at bottom.png" alt="Select Launch Instance at the bottom" width="900" />  
</p>  
* Do the same process over again but with the following exceptions (all which are under the Network settings section)
* Give a name that represents that this will be a private EC2 Server

* Select a Private Subnet
 <p align="center">  
  <img src="EC2 instance number 2 network settings select private subnet.png" alt="Select Private Subnet" width="900" />  
</p>  
 * Auto-assign public IP keep as disabled
 <p align="center">  
  <img src="EC2 instance number 2 network settings DISABLE auto-assign public ip.png" alt="Select Disable for AutoAssign IP" width="900" />  
</p>  
 * Select Create security group
 <p align="center">  
  <img src="EC2 instance number 2 network settings select creaste security group.png" alt="Select Create Security Group in Network Settings" width="900" />  
</p>  
   * Give your security group a name
 <p align="center">  
  <img src="EC2 instance number 2 network settings give securty group a name.png" alt="Give Security Group Name in Network Settings" width="900" />  
</p>  
   * Give your security group a description
 <p align="center">  
  <img src="EC2 instance number 2 network settings security group description.png" alt="Give your Security Group a Description" width="900" />  
</p>  
   * Under SSH change the Source type to Custom
 <p align="center">  
  <img src="EC2 instance number 2 network settings change to custom in ssh setting.png" alt="Change SSH source type." width="900" />  
</p>  
   * Under SSH change the Source to the Public Subnet created earlier
<p align="center">  
  <img src="EC2 instance number 2 network settings ssh source public subnet.png" alt="Change SSH Source" width="900" />  
</p>  


**CONNECT TO PUBLIC SERVER**

* Select the Public EC2 Instance recently created
<p align="center">  
  <img src="EC2 Select the EC2 Public Server recently created.png" alt="Select recently created public EC2 Instance" width="900" />  
</p> 
* Select Connect at top right
<p align="center">  
  <img src="EC2 Select Connect in top right corner.png" alt="Select Connect top right" width="900" />  
</p> 
* Select the EC2 Instance Connect Tab
<p align="center">  
  <img src="EC2 Select the EC2 Instance connect tab.png" alt="Select the EC2 Instance Connect tab" width="900" />  
</p> 
* Select Connect at the bottom
<p align="center">  
  <img src="EC2 Select connect at bottom .png" alt="Select Connect at the bottom" width="900" />  
</p> 
* An error message appears that "Failed to connect to your instance"
<p align="center">  
  <img src="EC2 error message when connecting to ec2 instance connect.png" alt="Error message connecting to EC2 Instance Connect" width="900" />  
</p> 
* The error occurs because the EC2 instance’s inbound security rules do not allow SSH traffic.
<p align="center">  
  <img src="EC2 reason for EC2 instance connect not working inbound rules status.png" alt="Reason for error message" width="900" />  
</p> 
* Search and Select Security Groups from AWS Searchbar
<p align="center">  
  <img src="EC2 select Securty group from AWS searchbar.png" alt="Select Security Group from AWS Searchbar" width="900" />  
</p> 
* Select the Public Security Group created from earlier
<p align="center">  
  <img src="EC2 Select public security group created from earlier.png" alt="Select Public Security Group created from earlier" width="900" />  
</p> 
* Select by scrolling down the inbound rules tab
<p align="center">  
  <img src="EC2 Select the inbound rules tab below.png" alt="Select Inbound Rules tab" width="900" />  
</p> 
* Select the edit inbound rules button
<p align="center">  
  <img src="EC2 edit inbound rules tab security group.png" alt="Select edit inbound rules buutton" width="900" />  
</p> 
* Select Add rule in edit inbound rules
<p align="center">  
  <img src="VPCSETUP add rule inbound security group.png" alt="Select Add rules button." width="900" />  
</p> 
* Select as the type SSH and the source anywhere ipv4
<p align="center">  
  <img src="EC2 set new security rule to SSH and anywhere ipv4.png" alt="Select new type and source" width="900" />  
</p> 
* Select Save Rules
<p align="center">  
  <img src="EC2 Select save rules for security groups.png" alt="Click Save Rules" width="900" />  
</p> 
* Repeat the steps above to connect to the EC2 Instance Connect and now connection can be established
<p align="center">  
  <img src="EC2 ec2 instance connect connection can be established.png" alt="Succesfully Established Connection" width="900" />  
</p> 

**Test Connectivity between EC2 Instances**

* Select from yourinstances the Private EC2 Instance created earlier

* Scroll down and copy the private ipv4 address

* Go back into your EC2 Instance connect terminal and type ping followed by the private ipv4 address that was just copied and press enter

* 








##### Contribution Policy

This project is not accepting external contributions, including pull requests or feature requests.

It serves as a personal archive of my learning journey in applying foundational concepts in software development and version control. Active development is not ongoing, and external changes will not be integrated.

Thank you for your understanding.
