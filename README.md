# Serverless exercises

Three excercises grouped in folders as delivered in Udemy course:
[AWS Certified Data Engineer Associate 2024](https://bravura.udemy.com/course/aws-data-engineer/learn/lecture/40305366#overview)

The excercises cover usage of AWS SAM with examples of Lambda, DynamoDB and API
Gateway.

## Pre-conditions

Make sure to have correctly configured AWS CLI with permissions to perform
required actions on right account.

## Folder structure

Each folder consisits:
- `commands.sh` - with list of shell commands to crete resources
- `template.yaml` - configuration of created resources
- folder `src` with relevant Python lambda code
- folder `gen` with generated yaml configuration `aws cloudformation package`
  command

Brief description of the folders:
- `project1`: deployment of only lambda function
- `project2`: modified lambda and API Gateway
- `project3`: as above, but with DynamoDB

## Usage

Execute in shell commands from `commands.sh` file.

Any above project folder could be used in any sequence. The most important is
to make sure that S3 bucket is created.

If case of doubts look at Section 6 'Compute' of the mentioned Udemy course.

## Possible errors

Creation of Python lambda might fail if too old version of Python is defined in
`template.yaml`
