# Project Infrastructure

## Architecturre Diagram
![Architecture](../screenshots/architecture_diagram.png)

## AWS cloud platform
### Database hosting on RDS (postgreSQL)
Database server is publicly accessible at `postgresql://postgres:password@udagram.xyz.us-east-1.rds.amazonaws.com/udagram`
### Web API Server hosted using Elastic Beanstalk service
Udagram web server is deployed using AWS Elastic Beanstalk service at `http://udagram-env-2.eba-xyz.us-east-1.elasticbeanstalk.com/`
### Frontend app hosted on S3 Bucket
Udagram frontend application is deployed using AWS S3 Bucket at `http://udagram-xyz.s3-website-us-east-1.amazonaws.com/home`
Users can access the Udagram application using the above link.
