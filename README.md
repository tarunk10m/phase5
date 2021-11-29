# phase5

Project: As a Full Stack Developer, you have to build a CI/CD pipeline to demonstrate continuous deployment and host the application on AWS EC2 instance.

As the project is in the final stage, management has asked you to automate the integration and deployment of the web application. You are required to set up an environment where the application will be hosted and accessed by users. The source code is supposed to be fetched from a GitHub repository.

Steps:
Creating an EC2 Instance:
From AWS ->open EC2 
-> instances 
-> Launch Instances 
Choose AMI-> selected the Amazon Linux 2 AMI 64-bit 
Choose Instance Type-> selected t2.micro 
Configure Instance Details 
Add Storage 
Add key pair and download it 
Launch

Connecting to EC2 via ssh:
Go to EC2 Dashboard -> Instances (Running) 
Select the instance 
Click connect 
Open ssh client tab and copy command
Open cmd from the downloaded location of key-pair and run the 
command. 

Hosting the springboot project
After connecting to the EC2. 
To access as main user run : sudo -i 
Install git using : yum install git -y 
Install maven using : yum install maven -y 
Clone the springboot project from github using : git clone ‘githublink’ 
Now go to the project directory 
Then run : mvn clean package 
Now to install docker run : yum install docker -y 
Now run : systemctl start docker 
Now to create an image for docker run the command : docker build -t 
springbootimage . 
After image is succesfully created run the command




Core Concepts:
Jenkins
Docker
Github
CI/CD
AWS



