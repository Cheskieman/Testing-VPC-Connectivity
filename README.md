# Testing-VPC-Connectivity...... 

## A complete step by step guide to test VPC Connectivity

* Connect to your Public Server from AWS Mamangement Console

* Test connectivity between your EC2 instances
 
* Test VPC connectivity with the internet.

### This project will demostrate how to 

* Set up a VPC & Network ACL


#### Step by Step Instructions guidance

**CREATE VPC & NETWORK ACL**

* Search and Select VPC from AWS Searchbar
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select Create VPC
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select VPC and more
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Give an specfic name in the auto-generation box.
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Scroll down and change the availibility zone number to one.
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Scroll down and click on arrow for Customize subnets CIDR blocks and input the ip addresses displayed in the two subnet boxes.
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Scroll doewn to where it says NAT Gateways and select the option for none.
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select Create VPC at bottom.
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select Network ACLs from the left hand navigation panel.
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select the Create network ACL on the top right
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Give your ACL a name
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select the earlier created VPC
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select Create Network ACL at the bottom.
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select the Subnet Asscociations tab
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select Edit Subnet Asscociations
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select the private subnet
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select Save Changes at bottom.
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select Security Groups from the left hand navigation panel
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select Create Security Group on the top right
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Give the Security Group a name.
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Give a decription for the Security Group
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select the earlier created VPC
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select add rule under Inbound rules
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select HTTP and anywhere IPV4 as both the type and source for the Inbound Rule
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  
* Select Create Security Group at the bottom.
<p align="center">  
  <img src="resources/EC2searchec2andselect.png" alt="Select Instance from AWS left-hand menu" width="900" />  
</p>  








##### Contribution Policy

This project is not accepting external contributions, including pull requests or feature requests.

It serves as a personal archive of my learning journey in applying foundational concepts in software development and version control. Active development is not ongoing, and external changes will not be integrated.

Thank you for your understanding.
