# awscli

## Installation
- RHEL
~~~
yum install awscli -y
aws --version  
~~~
- Ubuntu
To install the latest version of AWS CLI in Ubuntu, first, you'd have to install prerequisites using the following:
~~~
sudo apt install curl unzip
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
aws --version
~~~
## Configuration
- config: Contains all the information related to the configuration you made such as default region and type of default output.
- credentials: Contains access key and secret key as plain text.
~~~
aws configure
ls $HOME/.aws
aws ec2 describe-instances
~~~
## Tutorial

## Demo

## Use case


# AWS Knowledge
Understand the basic concept of the AWS service
**"Global AWS Infrastructure"** 
- Region
- Availability Zone (AZs)

**“AWS Services”** 
- Networking
  - VPC (Virtual Private Cloud)
  - SG (Security Group)
- Compute
  - EC2 (Elastic Compute Cloud)
- Storage
  - S3 (Simple Storage Service)
- Databases
  - RDS (Relational Database Service)
  - DynamoDB (MongoDB) Document Store
- Security
  - IAM (Identity & Access Management)


## AWS Certification
- Solution Architect, SysOps Administrator
## How to build your skills
- Do a project
  - YouTube
    - WordPress Website Hosting
    - Static Website Hosting
    - Serverless Web Crawler
  - Paid content (AWS Learning Learning Accelerator)
- Study AWS Architectures
  - AWS Reference Architectures
- Create your project ideas
  - ATO project
  - Fullstack App
  - Data Ingestion and processing pipeline
  - Anomaly detection dashboard
  - CI / CD pipeline
- Repeat Do a project
## Tips and Resources
- Join a community and read/ask questions
  - AWS subreddit
  - AWS version of Stack Overflow
- AWS Newsletters for staying current
- AWS Builders library for advanced cloud concepts

 
