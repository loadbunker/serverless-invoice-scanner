<<<<<<< HEAD
# Serverless Invoice Scanner Using AWS AI Services

## Project Overview

A serverless invoice processing application built using AWS cloud and AI services.

The application allows users to upload invoices, extract information using Amazon Textract, process extracted data using Amazon Bedrock, and store structured invoice records in Amazon DynamoDB.

## AWS Services

| Service | Purpose |
|---|---|
| Amazon S3 | Invoice storage |
| AWS Lambda | Serverless processing |
| Amazon Textract | Invoice data extraction |
| Amazon Bedrock | AI-powered data processing |
| Amazon DynamoDB | Invoice database |
| Amazon API Gateway | API management |
| Amazon Cognito | User authentication |
| AWS Amplify | Frontend hosting |
| Amazon Route 53 | Domain management |

## Architecture

The application follows an event-driven serverless architecture.

1. Users authenticate through Amazon Cognito.
2. Users upload invoices through the frontend.
3. Invoices are stored in Amazon S3.
4. AWS Lambda initiates invoice processing.
5. Amazon Textract extracts invoice information.
6. Amazon Bedrock processes the extracted information.
7. Structured invoice data is stored in DynamoDB.
8. Users retrieve invoice records through API Gateway.

## Project Structure

```text
serverless-invoice-scanner/
├── architecture/
├── frontend/
├── backend/
│   ├── generate-upload-url/
│   ├── start-processing/
│   ├── process-with-bedrock/
│   └── get-invoices/
├── infrastructure/
├── documentation/
└── README.md
```

## Project Status

Initial development.

Infrastructure deployment, implementation and testing are in progress.

## Learning Objectives

- AWS serverless architecture
- IAM and cloud security
- Event-driven processing
- AWS storage and databases
- API development
- AI service integration
- Cloud monitoring and troubleshooting

## Disclaimer

This project is intended for educational purposes. AWS services may incur charges depending on usage.
=======
# serverless-invoice-scanner
AI-powered serverless invoice processing using AWS Lambda, S3, Textract, Bedrock and DynamoDB.
>>>>>>> 7eab444c292a48e7fbc2a239e14fa0012d623a5e
