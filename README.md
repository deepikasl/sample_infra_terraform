### sample_infra_terraform

**Overview**:
This is a sample terraform project to bring up and destroy an AWS instance and helps you to understand how to provision Infrastructure using Terraform.

**Prerequisites/Requirements**:
- AWS EC2 account

**Instructions on using the sample project**
- Clone this project.
- Save your AWS credentials (Access Key ID and Secret Access Key) in `terraform.tfvars` file. you can go to [this](http://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSGettingStartedGuide/AWSCredentials.html) link to know how to get these.
 - Create a key pair for your AWS region using [this](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html) link. Download your pem key and paste it in `aws-ssh-key.pem`.
 - In `terraform.tfvars` put your AWS region that you selected in the above step.
 - Select an instance type suitable for your need from [this](https://aws.amazon.com/ec2/instance-types/) list and add it in `terraform.tfvars`.
 - Now to provision AWS instance you can enable this project on Shippable in `Infra` tab. Click on `Provision`, this should provision an EC2 instance on your selected AWS region.

**Instructions for setting up 3rd party services**
- [Setting up AWS EC2] (http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/get-set-up-for-amazon-ec2.html)

**Resources**
- [Documentation on provisioning Infrastructure using Terraform](http://docs.shippable.com/pipelines_configure/#provisioning-infrastructure-using-terraform)
