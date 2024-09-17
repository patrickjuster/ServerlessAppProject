<h1>AWS Serverless Reminder App</h1>

<h2>Description</h2>
The purpose of this project is to build a serverless reminder application on AWS. The premise of the application is that a pet cat can send a message to their owner's email. When the blue 'Email Minion' button is pressed, a command will be sent to API Gateway which will then send the message to the owner's email address.
<br />
<img src="https://i.imgur.com/5YqeB1u.png"/>
<br />
Assumptions based on the architecture initially had me under the impression that the project would be quick and easy. As I progressed through the project, it was truly illuminating seeing how much coding was necessary for the architecture to function properly. While the instructions did provide the code -- it was an eye opening experience that my coding skills will need some brushing up to get up to par with what's needed for architecting. As the project neared the end and I was ready to test the application, I ran into an error where the application was unable to fetch the data. Like in my current position I worked backwards to troubleshoot the issue. Researching online as well as reading through the project FAQ I was able to determine that I had misconfigured my Step Function. Starting from scratch I deleted the Step Function and followed the directions again -- resulting in a working application.
<br />
<br />
Reference: This project is based on Adrian Cantrill's mini-project: Pet-Cuddle-O-Tron 2023 (https://www.youtube.com/playlist?list=PLTk5ZYSbd9MgD5RMsUU-Vn5qRZY1A-UMU)
<br />
<br />
<h2>Arhitecture Example</h2>
<img src="https://i.imgur.com/sX5FzJQ.png"/>
<br />
<br />

<h2>AWS Services & Features Used</h2>

- <b>SES</b>
- <b>Lambda<b>
- <b>API Gateway</b>
- <b>S3 Static Website<b>
- <b>Step Functions<b>
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
