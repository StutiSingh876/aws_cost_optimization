# AWS Cost Optimization Using Lambda and EventBridge

## Project Overview

This project implements a serverless AWS cloud cost optimization workflow using AWS Lambda, EventBridge, IAM, and Python boto3 automation.

The system demonstrates how AWS services can be integrated to automate monitoring and optimization-related cloud operations without managing traditional servers.

---

## Technologies Used

* AWS Lambda
* Amazon EC2
* AWS IAM
* Amazon EventBridge
* Python
* boto3 SDK
* CloudWatch Logs

---

## Features

* Serverless AWS automation
* Scheduled execution using EventBridge
* IAM-based secure permission management
* Python boto3 AWS SDK integration
* Cloud resource monitoring workflow
* Cost optimization automation concepts

---

## Architecture

The workflow uses EventBridge to trigger a Lambda function periodically. The Lambda function executes Python boto3 scripts to interact with AWS resources and perform optimization-related actions.

### Architecture Flow

EventBridge → Lambda → boto3 → EC2 Resource Monitoring → Optimization Actions

---

## Project Structure

```bash id="zjlwmn"
aws-cost-optimization/
│
├── docs/
    ├── architecture.md
    ├──project_overview.md
├── screenshots/
│   ├── iam-roles.png
│   ├── iam-policies.png
├── .gitignore
├── README.md
│──lambds_function.py
│──requirements.txt

```

---

## Learning Outcomes

* Learned AWS serverless architecture
* Worked with AWS Lambda and EventBridge
* Understood IAM roles and policies
* Implemented automation using boto3
* Practiced AWS resource management workflows
* Understood cloud cost optimization concepts

---

## Future Improvements

* Add SNS notification integration
* Add CloudWatch monitoring metrics
* Extend automation to multiple AWS services
* Add Terraform-based infrastructure provisioning
* Add CI/CD pipeline integration

---

