# Secure Static Website Hosting Using AWS S3 and CloudFront

## Project Overview
This project demonstrates how to host a static website securely using Amazon S3 and Amazon CloudFront with Origin Access Control (OAC).

The S3 bucket remains private, while CloudFront delivers website content to users.

## AWS Services Used
- Amazon S3
- Amazon CloudFront
- Origin Access Control (OAC)
- AWS IAM
- AWS Billing and Cost Management

## Architecture
User → Amazon CloudFront → Origin Access Control → Private Amazon S3 Bucket

## Project Implementation

### 1. Create S3 Bucket
- Created an S3 bucket.
- Enabled Block Public Access.
- Uploaded the website file (index.html).

### 2. Configure CloudFront
- Created a CloudFront distribution.
- Configured the S3 bucket as the origin.
- Created Origin Access Control.
- Granted CloudFront permission to access the private S3 bucket.

### 3. Website Deployment
- Configured index.html as the default root object.
- Deployed the CloudFront distribution.
- Tested the website using the CloudFront domain.

### 4. Security Testing
- Verified that the CloudFront website was accessible.
- Tested direct S3 object access.
- Confirmed that direct S3 access returned AccessDenied.
- Kept S3 Block Public Access enabled.

### 5. Cache Management
- Created a CloudFront invalidation.
- Verified that its status became Completed.

## Project Results
- Successfully hosted a static website.
- Delivered website content through CloudFront.
- Kept the S3 bucket private.
- Implemented secure origin access using OAC.

## Skills Learned
- AWS S3 bucket management
- CloudFront distribution configuration
- Origin Access Control
- AWS security and permissions
- Static website deployment
- CDN cache invalidation

## Website URL
Add your CloudFront distribution URL here.

## Conclusion
Successfully implemented secure static website hosting using Amazon S3 and Amazon CloudFront with Origin Access Control.
