# DynamoDB Data Ingestion Project

## Overview

This project implements a data ingestion system for DynamoDB using DynamoDB Streams and AWS Lambda functions. The infrastructure is provisioned using Terraform, providing a scalable and efficient solution for processing and reacting to changes in DynamoDB tables.

## Components

- **Python:** Insert fake data on DynamoDB.
- **DynamoDB:** Set up DynamoDB tables for data storage.
- **DynamoDB Streams:** Enable DynamoDB Streams on tables to capture changes.
- **AWS Lambda Functions:** Process DynamoDB Stream events for data ingestion.
- **Terraform:** Provision infrastructure for DynamoDB, Lambda functions, and necessary IAM roles.

## Setup Instructions

1. **DynamoDB Setup:**
   - Create DynamoDB table(s) for data storage.
   - Enable DynamoDB Streams on the table(s) to capture changes.

2. **Lambda Functions:**
   - Write Lambda functions to process DynamoDB Stream events.
   - Ensure stateless functions with error handling and retry mechanisms.

3. **Data Processing Logic:**
   - Define logic for processing DynamoDB Stream events.
   - Handle inserts, updates, and deletes based on stream events.

4. **Terraform Infrastructure:**
   - Use Terraform scripts to provision infrastructure.
   - Define DynamoDB tables, Lambda functions, IAM roles, and policies.

5. **AWS Lambda Triggers:**
   - Configure Lambda functions as stream event triggers for DynamoDB.

6. **Error Handling and Logging:**
   - Implement logging within Lambda functions.
   - Use CloudWatch Logs for centralized logging.

7. **Security:**
   - Follow the principle of least privilege for IAM roles.
   - Secure sensitive information using AWS Secrets Manager or Parameter Store.

8. **Testing:**
   - Perform unit testing for Lambda functions.
   - Test the integration of DynamoDB Streams and Lambda.
   - Implement end-to-end testing for the entire data ingestion flow.

9. **Monitoring and Metrics:**
   - Set up CloudWatch Metrics for Lambda function invocations and errors.

10. **Deployment:**
    - Define a deployment strategy for Lambda functions.
    - Automate deployments using Github Actions.

11. **Documentation:**
    - Document the architecture, data flow, and deployment steps.
    - Include troubleshooting guides and best practices for developers.