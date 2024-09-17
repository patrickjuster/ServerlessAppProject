<h1>AWS Serverless Reminder App</h1>

<h2>Description</h2>
The purpose of this project is to build a serverless reminder application on AWS. The premise of the application is that a pet cat can send a message to their owner's email. When the blue 'Email Minion' button is pressed, a command will be sent to API Gateway which will then send the message to the owner's email address.
<br />
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


<h2>Project walk-through:</h2>
<br />
<br />
<p align="center">
Configure SES: <br/>
<img src="https://i.imgur.com/ps20U0H.png"/>
<br />
<br />
<br /> 
Add Lambda Function for Email & Configure:  <br/>
<img src="https://i.imgur.com/SvRJhPg.png"/>
 <img src="https://i.imgur.com/bFEoJl3.png"/>
 <img src="https://i.imgur.com/MIHwvA5.png"/>
 <img src="https://i.imgur.com/PIrKp7g.png"/>
 <img src="https://i.imgur.com/Q3uXD3F.png"/>
<br />
<br />
<br />
Configure State Machine: <br/>
<img src="https://i.imgur.com/W8AN8oQ.png"/>
 <img src="https://i.imgur.com/Qc2LAjH.png"/>
 <img src="https://i.imgur.com/Ll11JMc.png"/>
 <img src="https://i.imgur.com/LZep11B.png"/>
<br />
<br />
<br /> 
Implement API Gateway, API & Lambda Function:  <br/>
<img src="https://i.imgur.com/VRTab0l.png"/>
 <img src="https://i.imgur.com/pj3pr7S.png"/>
 <img src="https://i.imgur.com/EWW7icH.png"/>
 <img src="https://i.imgur.com/CQ5B1tP.png"/>
<br />
<br />
<br /> 
Implement Static Frontend & Test:  <br/>
<img src="https://i.imgur.com/ewWqLDI.png"/>
<img src="https://i.imgur.com/5VSjkoV.png"/>
<img src="https://i.imgur.com/8WQ5Vxu.png"/>
<img src="https://i.imgur.com/LLYPRJV.png"/>
<img src="https://i.imgur.com/SBPX1RM.png"/>
<img src="https://i.imgur.com/zsFdb4a.png"/>

<br />
<br />
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
