# Serverless Image Processing with S3 and Lambda

<br />

Final project for AWS Solutions Architect course on Manara[^1]  
Made by student: Omar Bamarouf

<br />

## 📋 Table of Content
- :pushpin: [Project Overview](#pushpin-project-overview)
- :triangular_ruler: [Architecture Diagram](#triangular_ruler-architecture-diagram)
- :wrench: [Component Details](#wrench-component-details)
- :sparkles: [Key Features](#sparkles-key-features)
- :cloud: [AWS Services Used](#cloud-aws-services-used)
- :rocket: [Why Serverless Architecture?](#rocket-why-serverless-architecture)
- :white_check_mark: [Conclusion](#white_check_mark-conclusion)

<br />

## :pushpin: Project Overview
This project presents a solution for a fully automated, event-driven image processing system using AWS serverless technologies.

It enables users to upload images (e.g., photos, product thumbnails) to an Amazon S3 bucket, which automatically triggers an AWS Lambda function to perform dynamic transformations such as resizing and watermarking. The processed images are then stored in a separate destination S3 bucket.

<br />

## :triangular_ruler: Architecture Diagram
![Architecture Diagram](architecture-diagram.png)

<br />

## :wrench: Component Details
| Component | Description |
| :--- | :--- |
| Original Images Bucket | Stores original images uploaded by users. Configured to trigger Lambda on uploads. |
| Image Processing Function | Processes images (resize and apply watermarks). |
| Processed Images Bucket | Stores processed images. |

<br />

## :sparkles: Key Features
- [x] **Event-Driven Processing** – Automatically triggers Lambda on S3 uploads.
- [x] **Image Transformations** – Resize and apply watermarks.
- [x] **Cost-Efficient** – Pay-per-use with Lambda & S3.
- [x] **Scalable** – Handles high traffic without manual scaling.

<br />

## :cloud: AWS Services Used
- **[Amazon S3](https://aws.amazon.com/s3/)** – Object storage service for scalable, secure, and durable file storage with high availability.
- **[AWS Lambda](https://aws.amazon.com/lambda/)** – Serverless compute service that runs code in response to events without managing servers.

<br />

## :rocket: Why Serverless Architecture?
This solution leverages AWS serverless architecture instead of traditional compute options for several key reasons:
1. Cost Efficiency
2. Automatic Scaling
3. Event-Driven & Decoupled
4. Reduced Operational Complexity
5. Faster Time-to-Market

<br />

## :white_check_mark: Conclusion
In this project, serverless architecture is the optimal choice for image processing, which are short-lived and sporadic workloads.

<br />

[^1]: Special thanks to Manara team for teaching me to become an AWS solutions architect.
