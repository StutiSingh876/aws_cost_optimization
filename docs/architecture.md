# Project Architecture

## Overview

This project uses a serverless AWS architecture to automate cloud cost optimization workflows.

The architecture is based on AWS Lambda, EventBridge scheduling, IAM permissions, and boto3-based AWS automation.

---

## Architecture Components

### 1. EventBridge

EventBridge acts as the scheduler for the automation workflow. It periodically triggers the Lambda function.

### 2. AWS Lambda

AWS Lambda executes the Python automation script without requiring server management.

### 3. boto3 SDK

The Lambda function uses boto3 to interact with AWS resources programmatically.

### 4. IAM Roles and Policies

IAM roles and policies provide secure permissions for Lambda to access AWS resources.

### 5. EC2 Monitoring

The automation logic monitors EC2-related resources for optimization workflows.

---

## Architecture Flow

EventBridge → Lambda Function → boto3 SDK → AWS Resource Monitoring → Optimization Workflow
+----------------------+
|   Amazon EventBridge |
|  (Scheduled Trigger) |
+----------+-----------+
           |
           v
+----------------------+
|     AWS Lambda       |
|  Python Automation   |
| (lambda_function.py) |
+----------+-----------+
           |
           v
+----------------------+
|      IAM Role        |
|  Permissions Policy  |
+----------+-----------+
           |
           v
+----------------------+
|   Amazon EC2 / EBS   |
|   Snapshot Handling  |
+----------------------+