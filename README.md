<h1>AWS Serverless Reminder App</h1>

<h2>Description</h2>
The purpose of this project is to demonstrate how to build a basic virtual private cloud (VPC) in AWS, connecting it to an existing VPC and troubleshooting issues. 
<br />
<br/>
The architecture of this VPC models a three-tiered web application structure -- containing 2 availability zones (AZ), three subnets per AZ, an internet gateway and a NAT gateway.
<br />
<br />
Note: This project is based on the AWS Skillbuilder lab, Amazon VPC Networking Basics. Project steps were followed on my personal AWS account and all screenshots are original.
<br />
<br />
<h2>Arhitecture Example</h2>
<img src="https://i.imgur.com/WtDBGzl.png"/>
<br />
<br />

<h2>AWS Services & Features Used</h2>

- <b>AWS VPC</b>
- <b>AWS EC2<b>
- <b>Transit Gateway</b>
- <b>Subnets<b>
- <b>Internet Gateway<b>
- <b>NAT Gateway<b>

<h2>Project walk-through:</h2>
<br />
<br />
<p align="center">
Create VPC: <br/>
<img src="https://i.imgur.com/LGk3VVq.png"/>
<br />
<br />
 <img src="https://i.imgur.com/zGYuWKN.png"/>
Launch EC2 Instance:  <br/>
<img src="https://i.imgur.com/f5yhzhc.png"/>
<br />
<br />
Testing Network Connectivity: <br/>
<img src="https://i.imgur.com/AdGYKTv.png"/>
<br />
<br />
Create a Transit Gateway:  <br/>
<img src="https://i.imgur.com/WBtoD1g.png"/>
<br />
<br />
Configure Attachments:  <br/>
<img src="https://i.imgur.com/H0hR0yw.png"/>
<br />
<br />
Configure Transit Gateway Routing:  <br/>
<img src="https://i.imgur.com/H0hR0yw.png"/>
<br />
<br />
<img src="https://i.imgur.com/lB3pk5m.png"/>
 <br />
 <br />
Retest connectivity between EC2 in VPC#1 & VPC#2:  <br/>
<img src="https://i.imgur.com/pETjSxV.png"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
