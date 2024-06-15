# Jenkins_Maven_Project
Deployed a simple java code on Tomcat server using Jenkins and Maven

 ![1_c63L9pm_Ty66m0Rh72vSsA](https://github.com/Faizan64/Jenkins_Maven_Project/assets/91891601/ffecc85a-6efc-4abf-9774-f285737e8936)


## Steps
- Install and configure Jenkins with AWS
- Install Maven
- Use Jenkins to install maven plugins
- With AWS ec2 setup the Tomcat sever
- Integrate Tomcat with Jenkins
- Build and deploy

- ## 2 EC2 instances for Jenkins and Tomcat 

![ec2 instances](https://github.com/Faizan64/Jenkins_Maven_Project/assets/91891601/86c62ace-9505-42d1-b035-5ce88555d427)

## Install and Configure Jenkins
- Create an ec2 instance and install and configure jenkins in the instance
- Since java is essential for jenkins first install jdk
- Documentation to install Jenkins on AWS :https://www.jenkins.io/doc/tutorials/tutorial-for-installing-jenkins-on-AWS.
- Jenkins uses port 8080 make sure to enable that in the instance and start using Jenkins
- Install all the plugins and start using jenkins
- 

![Jenkins dashboard](https://github.com/Faizan64/Jenkins_Maven_Project/assets/91891601/f9f8ec69-d66e-4a8d-aa75-093382c71992)

## Install Maven 
- Install maven on the Jenkins server
- First download the tar file from https://maven.apache.org/download.cgi unzip the tar file using tar -xvzf file-name
- In the .bash_profile file give maven and java path and now maven is configured and install in your server
- Install a maven plugin named maven integration and disable github sourch branch plugin.
- Maven is configured and Install on to your server
- Create a maven project Maven_project in jenkins and configure the pipeline by providing your github repo link.

## Setup Tomcat Server
- Launch an ec2 instance. Download the tar file from https://tomcat.apache.org/download-90.cgi and install tomcat server on to your instance
- Start the tomcat server. Provide new users in the tomcat-users.xml file and start using tomcat webserver.
- Now integrate Jenkins with tomcat
- Since the code is in java install jdk on tomcat server as well
- In Jenkins install a plugin named Deploy to container and the credentials of the tomcat server
- Create a maven project named Build_and_deploy_to_tomcat and after the configuration build the two projects

- ![Jenkins dashboard](https://github.com/Faizan64/Jenkins_Maven_Project/assets/91891601/f9f8ec69-d66e-4a8d-aa75-093382c71992)

## Deploy on tomcat 
- Completion of build and after integrating Jenkins with tomcat

 ![tomcat server](https://github.com/Faizan64/Jenkins_Maven_Project/assets/91891601/768d1a05-3a84-4df6-be8b-64ecd86cd814)

- A simple time tracker java code is deployed to tomcat server

![webserver](https://github.com/Faizan64/Jenkins_Maven_Project/assets/91891601/dfbdb531-2cfc-44f7-8c57-e841d51049b9)
