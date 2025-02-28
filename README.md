# AWS CLI Cheatsheet

## **AWS CLI Overview**
AWS Command Line Interface (CLI) is a tool that allows users to interact with AWS services from the command line.

---

## **AWS CLI Setup**
```sh
aws configure                   # Configure AWS CLI with credentials
aws --version                   # Check AWS CLI version
```

---

## **IAM (Identity and Access Management)**
```sh
aws iam list-users              # List all IAM users
aws iam create-user --user-name <username>  # Create a new IAM user
aws iam delete-user --user-name <username>  # Delete an IAM user
aws iam list-roles              # List all IAM roles
```

---

## **S3 (Simple Storage Service)**
```sh
aws s3 ls                       # List S3 buckets
aws s3 mb s3://<bucket-name>    # Create a new bucket
aws s3 cp <file> s3://<bucket>  # Upload a file to S3
aws s3 rm s3://<bucket>/<file>  # Delete a file from S3
aws s3 sync <local-dir> s3://<bucket>/  # Sync a local directory to S3
```

---

## **EC2 (Elastic Compute Cloud)**
```sh
aws ec2 describe-instances      # List all EC2 instances
aws ec2 start-instances --instance-ids <instance-id>  # Start an EC2 instance
aws ec2 stop-instances --instance-ids <instance-id>   # Stop an EC2 instance
aws ec2 terminate-instances --instance-ids <instance-id>  # Terminate an EC2 instance
```

---

## **Lambda (Serverless Functions)**
```sh
aws lambda list-functions       # List all Lambda functions
aws lambda invoke --function-name <function-name> output.txt  # Invoke a Lambda function
```

---

## **CloudFormation (Infrastructure as Code)**
```sh
aws cloudformation list-stacks  # List all CloudFormation stacks
aws cloudformation create-stack --stack-name <stack-name> --template-body file://template.json  # Create a stack
aws cloudformation delete-stack --stack-name <stack-name>  # Delete a stack
```

---

## **EKS (Elastic Kubernetes Service)**
```sh
aws eks list-clusters           # List all EKS clusters
aws eks describe-cluster --name <cluster-name>  # Get details of an EKS cluster
```

---

## **RDS (Relational Database Service)**
```sh
aws rds describe-db-instances   # List all RDS instances
aws rds stop-db-instance --db-instance-identifier <db-instance-id>  # Stop an RDS instance
aws rds start-db-instance --db-instance-identifier <db-instance-id>  # Start an RDS instance
```

---

## **CloudWatch (Monitoring & Logs)**
```sh
aws cloudwatch list-metrics     # List available CloudWatch metrics
aws logs describe-log-groups    # List all log groups
aws logs tail <log-group-name>  # Tail logs in real time
```

---

## **VPC (Virtual Private Cloud)**
```sh
aws ec2 describe-vpcs           # List all VPCs
aws ec2 describe-subnets        # List all subnets
aws ec2 describe-security-groups  # List security groups
```

---

## **Elastic Load Balancing (ELB)**
```sh
aws elb describe-load-balancers  # List all load balancers
aws elbv2 describe-target-groups  # List target groups for ALB/NLB
```

---

## **SNS (Simple Notification Service)**
```sh
aws sns list-topics             # List SNS topics
aws sns publish --topic-arn <topic-arn> --message "Hello World"  # Publish a message to an SNS topic
```

---

## **SQS (Simple Queue Service)**
```sh
aws sqs list-queues             # List all SQS queues
aws sqs send-message --queue-url <queue-url> --message-body "Test Message"  # Send a message to an SQS queue
```

---

## **Useful AWS CLI Resources**
- [AWS CLI Documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-services-overview.html)
- [AWS CLI Command Reference](https://docs.aws.amazon.com/cli/latest/reference/)
- [AWS Security Best Practices](https://aws.amazon.com/architecture/security-identity-compliance/)

---

This cheatsheet provides an extensive reference for AWS CLI commands across various services. Let me know if you have any suggestions or improvements!

