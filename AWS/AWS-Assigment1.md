# VPC & Networking

## Objective
Create a custom VPC with one public and one private subnet, set up the correct routing for internet access, and deploy EC2 instances across them.

## 1. Create the VPC

Custom VPC
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/create%20custom%20vpc.png" />

One public subnet
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/public%20subnet.png" />

One private subnet
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/private%20subnet.png" />

## 2. Internet Access

Create and attach an Internet Gateway
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/Internet%20gateway.png" />

Create an Elastic IP
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/elastic%20ip.png" />

Create a NAT Gateway in the public subnet
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/NAT%20gateway.png" />

## 3. Round tables

Public route table → default route via IGW
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/public%20route%20igw.png" />

Private route table → default route via NAT Gateway
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/Private%20route%20NAT.png" />

## 4. EC2 Instances 

Public EC2: launch in public subnet with public IP
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/Public%20EC2.png" />

Private EC2: launch in private subnet without public IP
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/Private%20EC2.png" />

## 5. Security 

Public EC2 SG: allow SSH/HTTP only from your IP
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/Security%20public%20Ec2%20sg.png" />

Private EC2 SG: allow only internal access (e.g. from public EC2 or Bastion host)
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/Security%20private%20Ec2%20sg.png" />
