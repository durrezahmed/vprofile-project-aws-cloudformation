# DevOps Project - AWS CloudFormation for Vprofile Project Stack Setup on Cloud

This is a DevOps Project using AWS CloudFormation for Vprofile Project Stack Setup on AWS Cloud.

[Link](https://github.com/durrezahmed/vprofile-project-devops) for vprofile app repository.

## Problem - Issues with Current Situation:

- High Cost in Maintaining Server with Storage

- Backup through AMI? Storage Cost

- Manual Setup is Time Consuming

- Chances of Human Error

## Solution - Fix:

- CloudFormation Ideal tool to Automate AWS Stacks

- Automatic Setup (No Human Errors)

- Maintain State of Infrastructure

- Version Control (IaC)

- Repeatable

- Reusable

## Tools used in the Project:

- [**AWS CloudFormation**](https://aws.amazon.com/cloudformation/) - Cloud Provisioning with Infrastructure as Code

- [**AWS Cloud Platform**](https://aws.amazon.com/) - Cloud Computing Resources

## About the Project:

- CI/CD Stack for Vprofile Project

- Jenkins

- Nexus

- SonarQube

- Tomcat, MySQL, Memcached, RabbitMQ

- With Data from S3 Bucket

## Steps:

1. Create S3 Bucket to upload Templates, create Folder named

   - `stack-template`

2. Note down Bucket name and Folder name

3. Create Key Pair

4. Write root template named `cicdtemp.yaml`

5. Write all Child Templates

   - `cicds3role.yaml`

   - `jenk.yaml`

   - `nexus.yaml`

   - `sonar.yaml`

   - `wintest.yaml`

   - `app01qa.yaml`

   - `db01qa.yaml`

6. Update Root template with Child Template Paths

7. Upload all Child Template to S3 Bucket in Folder

   - `stack-template`

8. Create Nested Stack by using `cicdtemp.yaml`
