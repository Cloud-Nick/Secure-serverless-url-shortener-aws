# Secure Serverless URL Shortener 

 

This project is a serverless web application built on AWS that allows authenticated users to generate shortened URLs. 

 

The goal of this project is to explore how serverless services can be combined to create a secure, scalable, and observable cloud application. 

 

 

## Architecture Overview 

 

The application is built using the following AWS services: 

 

- **AWS Lambda** – handles application logic 

- **API Gateway** – exposes HTTPS endpoints for the API 

- **DynamoDB** – stores shortened URL mappings 

- **Amazon Cognito** – provides authentication and user management 

- **CloudWatch** – logging and monitoring for application visibility 

 

This architecture removes the need for traditional servers and allows the application to scale automatically. 

 

 

## Project Goals 

 

This project focuses on several core cloud engineering concepts: 

 

- Building a **serverless application architecture** 

- Implementing **authentication and authorization** 

- Applying **least-privilege IAM policies** 

- Adding **logging and monitoring** for operational visibility 

- Understanding **scalable cloud design patterns** 

 

 

## High-Level Workflow 

 

1. A user authenticates using **Amazon Cognito**. 

2. The user submits a long URL through an **API Gateway endpoint**. 

3. The request triggers an **AWS Lambda function**. 

4. The Lambda function generates a shortened URL and stores the mapping in **DynamoDB**. 

5. When the shortened URL is accessed, another Lambda function retrieves the original URL and redirects the user. 

 

 

## Security Considerations 

 

Security practices explored in this project include: 

 

- Least-privilege IAM roles for Lambda functions 

- Authentication through Amazon Cognito 

- Logging and monitoring with CloudWatch 

- API Gateway authorization 

 

 

## Monitoring and Observability 

 

Operational visibility is provided through: 

 

- **CloudWatch Logs** for Lambda execution logs 

- **CloudWatch Metrics** for monitoring API usage and errors 

- Alerts for abnormal activity or failures 

 

 

## Future Improvements 

 

Planned improvements include: 

 

- Adding rate limiting and abuse protection 

- Implementing infrastructure deployment using Terraform or CloudFormation 

- Adding a simple frontend interface 

- Implementing custom domain support 

 

 

## Learning Outcomes 

 

Through this project I am gaining hands-on experience with: 

 

- serverless application design 

- AWS security and identity management 

- cloud monitoring and logging 

- designing scalable cloud architectures 

 
