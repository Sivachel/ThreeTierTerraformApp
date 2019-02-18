# Terraform Three tier App

## Description

- Three tier app which consists of a React app which provides the view, the Node app to provide the logic and  a MongoDB server for our database.
- React App will be deployed into the S3 bucket, whereas the Node app and the MongoDB will be running as an EC2 instance.

## Requirements

- Local machine should have the following installed in order to get the app working and deploy successfully on AWS
  - Terraform
  - Python
  - Pip
  - AWS CLI

## Instructions

#### Exporting AWS Keys

``export AWS_ACCESS_KEY_ID=your_key_here``

``export AWS_SECRET_ACCESS_KEY=your_key_here``

In order to access the AWS with the correct credentials, the keys must be exported in the terminal

#### Terraform

``terraform init``

The terraform init command is used to initialize a working directory containing Terraform configuration files. This is the first command that should be run after writing a new Terraform configuration or cloning an existing one from version control. It is safe to run this command multiple times.

``terraform plan``

The terraform plan command is used to create an execution plan. Terraform performs a refresh, unless explicitly disabled, and then determines what actions are necessary to achieve the desired state specified in the configuration files.

This command is a convenient way to check whether the execution plan for a set of changes matches your expectations without making any changes to real resources or to the state. For example, terraform plan might be run before committing a change to version control, to create confidence that it will behave as expected.

``terraform apply``

The terraform apply command is used to apply the changes required to reach the desired state of the configuration, or the pre-determined set of actions generated by a terraform plan execution plan.