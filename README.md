# DevOpsAWSChallenge


For this challenge I created a custom VPC and attached an internet gateway to it. I then created three subnets, two private and one public. I then created two route tables, one for the public subnet and another to the private. < security rules>

I set up a mysql Amazon rds and selected the option that disallowed access to the internet.

Security groups for the ec2 and the rds. security rules
Security rules

# Improvements

To achieve the MVP I did cut corners on the password and security rules, and if I had extra time I would go back and fix these. I did not use an environment variable for the password in the app.py file. I also created a security rule that allowed traffic on all ports, where I only needed port 5000 open. This effectively defeated the purpose of the security group.  I did this because I was unsure how to use nginx and I didn’t want to run unto security issues whilst I was still learning about it.


This project involved creating a custom VPC, a public subnet and a private subnet. 

An EC2 instance runs inside the public subnet with its own security group, and the 

![Diagram](https://github.com/mauvesky1/DevOpsAWSChallenge/blob/main/ImageFiles/Diagram.png)




The final result:
![Final]