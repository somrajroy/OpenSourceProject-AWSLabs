#### This repository contains code which can be used as "user data" while creating AWS EC2 instances for Client Demo's, POC's and doing hands on Labs. <br/>
<br/>
* These scripts should be used for Client Demo's, POC's and labs for setting up a scaled and load-balanced application, Demo of EC2 Auto Scaling, elasticity, High availability, Load balacing etc.. <br/>
* These scripts will install an Apache web server (httpd) and would display the private IP and avilability zones of the EC2 instances. If refreshed few times it can be seen that the load is routed to different EC2 servers in different availability zones. <br/>
* They are very useful while testing autoscaling/HA scenarios. A webserver will be installed and will display its AZ & IP (other required meta data can be easily added)<br/>
* CPU load on the servers can be increased by executing "stress --cpu 4 --timeout 300" <br/>
* An alarm can be triggered, when CPU Load exceeds a certain value, which will inform ASG to scale out <br/>
* After a few minutes, the number of instances will increase under EC2 console (or ASG > Instance Management). It enacts the scale-out policy. <br/>
* After few minutes more, the stress test will stop and the ASG enacts the scale-in policy.<br/>
* There are 3 scripts for (AWS) Linux, Windows 2016 and Windows 2019 servers <br>
* These scripts can be extended with minor changes and can be used for most of the hands on Labs for AWS Solution Architect certifications (SAA & SA Pro).<br/>

#### Sample Architectures that can be are built for Demo's : <br/>

![image](https://user-images.githubusercontent.com/92582005/202110301-09cda5b0-4f4f-4324-b3ac-e62ad5322b65.png) <br/>

![image](https://user-images.githubusercontent.com/92582005/202110446-6e49b105-8e2c-45d4-9a5e-741719aa0aad.png) <br/>
