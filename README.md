# Creating-an-S3-Lifecycle-Policy
Hands-on AWS lab that demonstrates how to create an S3 bucket and configure lifecycle policies to transition objects between storage classes, delete expired data, and clean up incomplete multipart uploads for cost optimization.
# Creating an S3 Lifecycle Policy

## Lab Overview

In this lab, you will create an Amazon S3 bucket and configure a **Lifecycle Policy** to automatically manage objects stored in the bucket.

You will learn how to:
- Create an S3 bucket with required configurations
- Define lifecycle rules for storage class transitions
- Automatically delete expired objects
- Clean up incomplete multipart uploads

Lifecycle policies help optimize storage costs and maintain data hygiene.

## Prerequisites

- AWS Account
- AWS CLI installed and configured
- IAM user/role with:
  - AmazonS3FullAccess (or equivalent permissions)
- Basic knowledge of AWS S3

---


## Lab Tasks

### Task 1: Create an S3 Bucket

The bucket will be created with:
- A globally unique name
- Specified AWS region
- Private ACL

### Task 2: Create a Lifecycle Policy

The lifecycle rule will:
- Transition objects to **STANDARD_IA** after 30 days
- Transition objects to **GLACIER** after 90 days
- Permanently delete objects after 365 days
- Abort incomplete multipart uploads after 7 days

---
## Steps

### Step 1: Clone the Repository
Step 2: Create the S3 Bucket
Step 3: Apply the Lifecycle Policy
Step 4: Verify the Lifecycle Rule

### Outcome

S3 bucket successfully created

Lifecycle rule enabled

Objects automatically transitioned and expired based on rule configuration

## Best Practices

Test lifecycle rules in non-production buckets

Monitor lifecycle transitions using S3 Storage Lens

Avoid conflicting lifecycle rules

### References

AWS S3 Lifecycle Rules Documentation

AWS S3 Storage Classes Overview
