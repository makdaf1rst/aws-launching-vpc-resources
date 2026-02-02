<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Launching VPC Resources

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-ec2)

**Author:** saqibh49@gmail.com  
**Email:** saqibh49@gmail.com

---

## Launching VPC Resources

![Image](http://learn.nextwork.org/grateful_white_lucky_bat/uploads/aws-networks-ec2_8ee57662)

---

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is a basically a separate bubble within the AWS ecosystem that allows for storing resources and data without it being out on the open web

### How I used Amazon VPC in this project

I used Amazon VPC to create public and private spaces (subnets) to store and access resources and data. 

### One thing I didn't expect in this project was...

One thing I didn't expect in this project was how much faster and simpler it is to set up a VPC and all its components with the VPC and More option.

### This project took me...

This project took me 20 minutes

---

## Setting Up Direct VM Access

Directly accessing a virtual machine means logging into the OS of the virtual machine and using it like its the computer in front of me. This is used for deeper level admin work for example. 

### SSH is a key method for directly accessing a VM

SSH is a type of traffic used to connect to virtual machines. Once I connect to my virtual machine via SSH, all data going between the 2 is encrypyted. 

### To enable direct access, I set up key pairs

Key pairs are a way of securely connecting to an instance. The public key stays with the virtual machine and the private key sstays with me, the user. When I want to login, the only thing that can unlock the instance is the private key in my possession. 

A private key's file format means essentially the file type that the key is saved within. My private key's file format was .pem

---

## Launching a public server

I had to change my EC2 instance's networking settings by changing the VPC to my nextwork vpc and the subnet to my public subnet under network settings. 

![Image](http://learn.nextwork.org/grateful_white_lucky_bat/uploads/aws-networks-ec2_88727bef)

---

## Launching a private server

My private server has its own dedicated security group because the rules of who can access instances in my public server are completely different who can access resources in my private server. I don't want just anyone from the internet to be able to see sensitive, private info from my private server.

My private server's security group's source is my public security group which means only resources from my public server can access items in my private server. 

![Image](http://learn.nextwork.org/grateful_white_lucky_bat/uploads/aws-networks-ec2_4a9e8014)

---

## Speeding up VPC creation

I used an alternative way to set up an Amazon VPC! This time, I used the VPC and More option to create my VPC, subnets, and internet gateways all at once.

A VPC resource map is a diagram of all the pieces within a VPC and how they connect. 

My new VPC has a CIDR block of 10.0.0.0/16. It is possible for my new VPC to have the same IPv4 CIDR block as my existing VPC because VPCs are inherently separate and only interact if directed to do so. 

![Image](http://learn.nextwork.org/grateful_white_lucky_bat/uploads/aws-networks-ec2_1cbb1b88)

---

## Speeding up VPC creation

### Tips for using the VPC resource map

When determining the number of public subnets in my VPC, I only had two options 0 and 2. This was because of the number of regions my VPC would be stored in. 

The set up page also offered to create NAT gateways, which are a secure way for private subnets to access the internet without the use of public IP addresses. 

![Image](http://learn.nextwork.org/grateful_white_lucky_bat/uploads/aws-networks-ec2_8ee57662)

---

---
