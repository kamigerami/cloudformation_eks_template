#### Cloudformation ECS template

This will create:

- IAM Role
- VPC
- EKS Nodes

Using CloudFormation templates and the AWS CLI

##### 1. Create IAM Role
```
aws cloudformation create-stack --stack-name myEKS-$(openssl rand -hex 12) --template-body file://iam.yaml --region us-east-1 --capabilities CAPABILITY_IAM
```
