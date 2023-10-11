# Project: Cloud Server Test - AWS
## Authors: Samaad Turner
# Problem Domain
Deploy a basic server to AWS Elastic Beanstalk.

# Links and Resources
GitHub Actions ci/cd
GUI URL: http://cf-web-service-env.eba-ivu2hrmn.us-west-2.elasticbeanstalk.com/bikes
CLI Deploy url: http://cloud-service-cli-env.eba-up6trdbs.us-west-2.elasticbeanstalk.com/bikes
# Collaborators

# Setup
Processes
For GUI deployment:

1. Create Environment
2. Application Name (can be same as others)
3. Environment Name (can left be default)
4. Platform - Node.js
5. Platform Branch - Node.js 18 ~ Version 5.8.2 (recommended)
6. Upload your code - give version name & local file, upload zip (including Json & server.js DO NOT NAME INDEX.JS)
7. Single Instance (default)
8. Exisiting Service Role: aws-elasticbeanstalk-service-role
9. EC2 instance profile: aws-elasticbeanstalk-ec2-role
10. Skip to Review, and Deploy!
    
For CLI deployment:

1. eb init in terminal
2. use default names, select a region, answer No to options
3. After making sure you ACP to Github, eb create
4. default names, select region, answer No to options
5. create auto deploys but if you make changes to code base ACP to Github & then eb deploy
   
# Routes
* / ~ Proof of life route
* /Hello?Name=<name> ~ Proof of life with query
  
# Tests
To run tests, after running npm i, run the command npm test