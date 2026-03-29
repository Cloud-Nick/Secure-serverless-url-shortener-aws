🚀 Secure Serverless URL Shortener

This project is a serverless web application built on AWS that allows authenticated users to generate and use shortened URLs.

The goal of this project is to demonstrate how core AWS services can be combined to build a secure, scalable, and production-style application without managing traditional servers.

🧠 Architecture Overview

The application is built using the following AWS services:

AWS Lambda – handles backend application logic
API Gateway / Lambda Function URL – exposes HTTPS endpoints
DynamoDB – stores URL mappings
Amazon Cognito – handles user authentication and session management
CloudWatch – provides logging and monitoring

This serverless architecture eliminates the need for infrastructure management and automatically scales based on usage.

🎯 Project Goals

This project focuses on building practical cloud engineering skills, including:

Designing and implementing a serverless architecture
Integrating authentication using Amazon Cognito
Applying least-privilege IAM principles
Implementing logging and monitoring for visibility
Understanding scalable and event-driven system design
🔄 High-Level Workflow
A user signs in via Amazon Cognito
The frontend sends a request to create a short URL
The request triggers an AWS Lambda function
The Lambda function generates a unique short ID and stores it in DynamoDB
When a short URL is accessed, a Lambda function retrieves the original URL
The user is redirected to the original destination
🔐 Security Considerations

This project incorporates several foundational security practices:

Least-privilege IAM roles for all Lambda functions
Authentication and access control using Amazon Cognito
Controlled API access through Gateway / Function URL configuration
Logging for auditing and debugging
📊 Monitoring & Observability

Operational visibility is implemented using:

CloudWatch Logs – for Lambda execution and debugging
CloudWatch Metrics – for tracking usage and errors
Basic monitoring to identify failures and abnormal behavior
🛠️ Future Improvements

Planned enhancements include:

Custom domain support for cleaner short URLs
Rate limiting and abuse protection
Infrastructure as Code (Terraform or CloudFormation)
Improved frontend user experience
Analytics (click tracking, usage metrics)
📚 Learning Outcomes

Through this project, I am gaining hands-on experience with:

Serverless application design
AWS identity and access management
Cloud monitoring and debugging
Building scalable, event-driven systems
