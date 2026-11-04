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
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/Internet%20gateway.png />

Create an Elastic IP
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/elastic%20ip.png" />

Create a NAT Gateway in the public subnet
<img src="https://github.com/pmoh1999/screenshots/blob/656edca2ce201edb5e44f661095950b896f9870a/shots/NAT%20gateway.png" />