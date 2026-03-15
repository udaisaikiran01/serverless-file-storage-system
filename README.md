# Serverless File Storage System

A full-stack serverless cloud application that allows users to upload, list, and download files through a web interface.

The system is built using AWS serverless services and follows a cloud-native architecture.

## Live Demo
http://serverless-file-ui-udai.s3-website.eu-north-1.amazonaws.com

## Features
- Upload files through a browser interface
- View list of uploaded files
- Download files securely using pre-signed URLs
- Fully serverless architecture

## Architecture

Browser  
↓  
S3 Static Website (Frontend UI)  
↓  
API Gateway  
↓  
AWS Lambda  
↓  
Amazon S3 (File Storage)  
↓  
Amazon DynamoDB (Metadata)

## Technologies Used

- AWS Lambda
- Amazon API Gateway
- Amazon S3
- Amazon DynamoDB
- HTML
- CSS
- JavaScript

## API Endpoints

POST `/upload`  
Upload a file.

GET `/files`  
Retrieve list of uploaded files.

GET `/download/{fileId}`  
Generate a secure pre-signed download URL.

## Future Improvements

- Authentication for users
- File size restrictions
- Drag-and-drop file upload UI
- HTTPS via CloudFront
