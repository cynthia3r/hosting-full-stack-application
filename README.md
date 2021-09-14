# Udagram

The udagram application includes all the major components of a Full-Stack web application and the task was to
* make the necessary changes in code to connect to the AWS RDS database and S3 storage service
* deploy and host the application to AWS cloud platform
* build a seamless CI/CD pipeline which is well documented and maintainable

## Getting Started

1. Clone this repo locally into the location of your choice. [GitHub repo](https://github.com/udacity/nd0067-c4-deployment-process-project-starter) 
1. Move the content of the udagram folder at the root of the repository as this will become the main content of the project.
1. Open a terminal and navigate to the root of the repo
1. follow the instructions in the installation step

### Dependencies
Project dependencies can be found [here](./docs/APP_DEPENDENCIES.md)

### Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. `postgresql://postgres:postgres@udagram-db.c7cjjx4qtzlu.us-east-1.rds.amazonaws.com:5432/postgres`
1. In AWS, provision a s3 bucket for hosting the uploaded files. `http://udagram-frontend-media-bucket.s3-website-us-east-1.amazonaws.com/`
1. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.
1. From the root of the repo, navigate udagram-api folder `cd starter/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
1. Without closing the terminal in step 1, navigate to the udagram-frontend `cd starter/udagram-frontend` to intall the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Infrastructure and Architecture Diagram
Project infrastructure details can be found [here](./docs/INFRASTRUCTURE.md)

## CI/CD Pipeline
Project pipeline process can be found [here](./docs/PIPELINE_PROCESS.md)


## AWS and CircleCI Configuration screens and settings
![RDS DB Instance](./screenshots/aws_rds_db_instance.png)
![EB Backend Server Health](./screenshots/aws_eb_backend_api_health.png)
![Frontend S3 Bucket](./screenshots/aws_frontend_media_s3_bucket.png)
![CircleCI Environment Variables](./screenshots/circleci_env_variables.png)
![CircleCI GitHub Integration and Deploy Pipeline](./screenshots/circleci_build_success.png)

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## Frontend and backend API URLs
- Udagram Backend API URL: `http://udagramapi-env.eba-apmqumk3.us-east-1.elasticbeanstalk.com/api/v0`
- Udagram Frontend URL: `http://udagram-frontend-media-bucket.s3-website-us-east-1.amazonaws.com/`

## License

[License](LICENSE.txt)