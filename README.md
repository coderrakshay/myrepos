# aYo tech-test
This project is contains the project files for the aYo DevopsEngineer assignment. I'm not 100% satisfied with the results, and would have loved to spend more time on some of the points below.


## Web Application
- Apache Tomcat docker container 9: http://3.89.108.255:8080/
- sample.war app URL: http://3.89.108.255:8080/sample/

## SSL/TLS Offload
- Configured SSL via EC2 instance fpor port 8080 and 443
- Created self-signed certificate
- unable to apply certificates on EC2

## Storage
- S3 bucket ARN: arn:aws:s3:::ayos3logdestination
- IAMRole "ec2RoleS3Access" created with permission to write
- Unable to get Tomcat logs to write to S3, considered using CloudWatch, but thats not block storage.

## EC2 instances configured
- Node 1: Linux Docker host running apache tomcat and sample app
- Node 2: Linux Jenkins server, not running, unable to setup enviornment, irritating JDBC error with starting up Jenkins

## URL Shortening Service
- Created and can be found under filename: https://github.com/thefran42/aYo_TechTest/blob/main/URL_Shortening_Service_Architectural_Diagram.drawio

## License and Authors
- Authors: Francois Conradie
- Date 2021/11/19
