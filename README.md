# AWS Static Website Deployment

## Project Overview

This project demonstrates the deployment of a static website using
Amazon S3, CloudFront, Route 53, AWS Certificate Manager and
Origin Access Control.

## Architecture

![AWS Architecture](architecture/architecture.png)

## AWS Services Used

- Amazon S3
- Amazon CloudFront
- Amazon Route 53
- AWS Certificate Manager
- Origin Access Control (OAC)

## Architecture Flow

User
↓
Route 53
↓
CloudFront
↓
Origin Access Control
↓
Amazon S3
↓
index.html

## Implementation

### 1. Amazon S3

Created an S3 bucket and uploaded the static website files.

### 2. CloudFront

Created a CloudFront distribution with S3 as the origin.

Configured CloudFront with:

- HTTPS
- Origin Access Control
- Default root object: index.html

### 3. Origin Access Control

Configured OAC so CloudFront can securely access the S3 bucket.

### 4. Route 53

Configured Route 53 to point the custom domain to CloudFront.

### 5. SSL Certificate

Configured HTTPS using AWS Certificate Manager.

## What I Learned

- S3 static website deployment
- CloudFront CDN
- Route 53 DNS
- HTTPS and SSL certificates
- Origin Access Control
- AWS troubleshooting
- DNS configuration
- 
