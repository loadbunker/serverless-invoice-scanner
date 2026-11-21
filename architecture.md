# AWS Architecture Documentation

## 1. Overview

The Serverless Invoice Scanner is designed using AWS serverless services to automate invoice processing.

The architecture consists of two major components:

- Frontend / Static Hosting
- Backend Processing

## 2. AWS Services and Responsibilities

### Amazon Route 53
Responsible for domain management and routing users to the application.

### AWS Amplify
Hosts the frontend application and provides the interface through which users interact with the system.

### Amazon Cognito
Handles user authentication, including registration and login.

### Amazon API Gateway
Acts as the communication layer between the frontend and backend Lambda functions.

### Amazon S3
Stores uploaded invoice documents.

### AWS Lambda
Executes backend processing without requiring server management.

The architecture uses multiple Lambda functions for different responsibilities.

### Amazon Textract
Extracts text and structured information from uploaded invoices.

### Amazon Bedrock
Processes extracted invoice information using AI to identify and structure relevant pricing information.

### Amazon DynamoDB
Stores processed invoice information and supports invoice retrieval.

## 3. Invoice Processing Workflow

1. Users access the application through Route 53.
2. AWS Amplify serves the frontend.
3. Amazon Cognito authenticates users.
4. API Gateway handles frontend API requests.
5. Users upload invoices to Amazon S3.
6. S3 triggers an AWS Lambda function.
7. Lambda initiates invoice text extraction using Amazon Textract.
8. Another Lambda function processes the extracted information.
9. Amazon Bedrock helps extract and structure pricing information.
10. Processed invoice information is saved in DynamoDB.

## 4. Invoice Retrieval Workflow

1. Users request previously processed invoices.
2. API Gateway receives the GET request.
3. API Gateway invokes the retrieval Lambda function.
4. Lambda queries DynamoDB.
5. Invoice information is returned to the frontend.

## 5. Architecture Benefits

- Serverless infrastructure.
- Reduced server administration.
- Event-driven processing.
- Scalable document storage.
- AI-powered invoice processing.
- Managed user authentication.
- Structured database storage.

## 6. Project Status

Architecture documentation created.

AWS service implementation and integration are planned as subsequent development milestones.
