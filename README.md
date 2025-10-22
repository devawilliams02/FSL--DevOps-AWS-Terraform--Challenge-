## Project: RDICIDR

This repository contains Terraform configurations to deploy the RDICIDR static website with S3 and CloudFront across multiple environments.

### Environment Distributions

| Environment | CloudFront URL |
|------------|----------------|
| Development (devel) | [https://d20mvsazi9b2gs.cloudfront.net/](https://d20mvsazi9b2gs.cloudfront.net/) |
| Staging (stage)     | [https://d2pww1cda85r89.cloudfront.net/](https://d2pww1cda85r89.cloudfront.net/) |
| Production (prod)   | [https://d14pzqfz8qx8ao.cloudfront.net/](https://d14pzqfz8qx8ao.cloudfront.net/) |

### Notes

- All environments use **S3 for website hosting** and **CloudFront for CDN**.  
- Access to S3 buckets is restricted to CloudFront only via **Origin Access Identity (OAI)**.  
- Logging is enabled for all distributions to monitor access.  
- Buckets are versioned to keep track of changes to website content.
