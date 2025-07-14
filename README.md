# Serverless Image Processing with S3 and Lambda
Final project for AWS Solutions Architect Course on Manara[^1]  
Solution made by student: Omar Bamarouf

<br />

## Table of Content
- [Project Overview](#project-overview)
- [Architecture Diagram](#architecture-diagram)
- [Component Details](#component-details)
- [AWS Services Used](#aws-services-used)
- [Key Features](#key-features)
- [Why Serverless Architecture?](#why-serverless-architecture)
- [Conclusion](#conclusion)

<br />

## Project Overview
This project presents a solution for serverless image processing where users can upload images to an S3 bucket, triggering an AWS Lambda function that resizes, applies watermark, and stores processed images in another S3 bucket.

<br />

## Architecture Diagram
![Architecture Diagram](architecture-diagram.png)

<br />

## Component Details
| Component | Description |
| :--- | :--- |
| Original Images Bucket | Stores original images uploaded by users. Configured to trigger Lambda on uploads. |
| Image Processing Function | Processes images (resize and apply watermarks). |
| Processed Images Bucket | Stores processed images. |

<br />

## AWS Services Used
- **Amazon S3** – Object storage service for scalable, secure, and durable file storage with high availability.
- **AWS Lambda** – Serverless compute service that runs code in response to events without managing servers.

<br />

## Key Features
- [x] **Event-Driven Processing** – Automatically triggers Lambda on S3 uploads.
- [x] **Image Transformations** – Resize and apply watermarks.
- [x] **Cost-Efficient** – Pay-per-use with Lambda & S3.
- [x] **Scalable** – Handles high traffic without manual scaling.

<br />

## Why Serverless Architecture?
This solution leverages AWS serverless architecture instead of traditional compute options for several key reasons:
1. Cost Efficiency.
2. Automatic Scaling.
3. Event-Driven & Decoupled.
4. Reduced Operational Complexity.
5. Faster Time-to-Market.

<br />

## Conclusion
In this project, serverless architecture is the optimal choice for image processing, which are short-lived and sporadic workloads.

<br />

[^1]: Special thanks to Manara team for teaching me to become an AWS solutions architect.
