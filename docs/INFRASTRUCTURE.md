# Project Infrastructure

## Architecture Diagram
![Architecture](../screenshots/architecture_diagram.png)

## AWS cloud platform
### Database hosting on RDS (postgreSQL)
Database server is publicly accessible at `postgresql://postgres:postgres@udagram-db.c7cjjx4qtzlu.us-east-1.rds.amazonaws.com:5432/postgres`
### Web API Server hosted using Elastic Beanstalk service
Udagram web server is deployed using AWS Elastic Beanstalk service at `http://udagramapi-env.eba-apmqumk3.us-east-1.elasticbeanstalk.com/`
### Frontend app hosted on S3 Bucket
Udagram frontend application is deployed using AWS S3 Bucket at `http://udagram-frontend-media-bucket.s3-website-us-east-1.amazonaws.com/`
Users can access the Udagram application using the above link.
