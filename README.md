# Automation with CloudFormation

## Activity Overview

Deploying infrastructure in a consistent, reliable manner is challenging. AWS CloudFormation addresses this by defining infrastructure in a template that can be automatically deployed, even on an automated schedule. This lab provides experience in deploying and editing CloudFormation stacks, offering an interactive experience to consult documentation and discover how to define resources within a CloudFormation template.

## initial-template:
![initial-template](https://github.com/Mohamed-kittany/Canvas-Lab-190-AutomatingDeploymentsWithAWSCloudFormation/assets/161580792/abaab4dd-0286-4dec-b249-1fb8d5dbdea4)

## Activity Objectives

After completing this lab, I was able to:
- Deploy an AWS CloudFormation stack with a defined Virtual Private Cloud (VPC) and Security Group.
- Configure an AWS CloudFormation stack with resources such as an Amazon Simple Storage Service (S3) bucket and Amazon Elastic Compute Cloud (EC2) instance.
- Terminate an AWS CloudFormation stack and its respective resources.

## Tasks Completed

### Task 1: Deploy a CloudFormation Stack
- **Objective:** Deploy a CloudFormation stack that creates a VPC and Security Group.
- **Actions:**
  - Downloaded and reviewed the `task1.yaml` template file.
  - Uploaded the template to CloudFormation and created a stack named "Lab."
  - Monitored the stack creation process through the Events and Resources tabs.
  - Verified the creation of the VPC and Security Group in the VPC console.

### Task 2: Add an Amazon S3 Bucket to the Stack
- **Objective:** Add an Amazon S3 bucket to the existing CloudFormation stack.
- **Actions:**
  - Edited the `task1.yaml` template to include an Amazon S3 bucket.
  - Used the AWS CloudFormation documentation for S3 template snippets.
  - Updated the stack with the revised template.
  - Verified the creation of the S3 bucket in the S3 console.

### Task 3: Add an Amazon EC2 Instance to the Stack
- **Objective:** Add an Amazon EC2 instance to the existing CloudFormation stack.
- **Actions:**
  - Added a parameter for the Amazon Linux 2 AMI ID using AWS Systems Manager Parameter Store.
  - Updated the template to define an EC2 instance with properties for ImageId, InstanceType, SecurityGroupIds, SubnetId, and Tags.
  - Used the AWS CloudFormation documentation for EC2 instance template snippets.
  - Updated the stack with the revised template.
  - Verified the creation of the EC2 instance in the EC2 console.

### Task 4: Delete the Stack
- **Objective:** Delete the CloudFormation stack and its resources.
- **Actions:**
  - Selected the "Lab" stack in the CloudFormation console and initiated the deletion process.
  - Verified the deletion of the stack and its resources (S3 bucket, EC2 instance, and VPC).

## What I Have Achieved/Learned from this Lab
- Gained experience in deploying AWS CloudFormation stacks.
- Learned how to add and configure resources within a CloudFormation template.
- Successfully added an Amazon S3 bucket and EC2 instance to an existing stack.
- Understood how to use AWS Systems Manager Parameter Store to dynamically retrieve AMI IDs.
- Gained skills in updating and managing CloudFormation stacks through the AWS Management Console.

