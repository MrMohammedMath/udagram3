## Udagram Infrastructure

![Architecture](architecture.png)

### AWS
#### RDS Postgres
For storing and retrieving data, the application server makes use of the AWS RDS Postgres database.

Database Endpoint: `postgres.ctjskkcomkti.eu-central-1.rds.amazonaws.com`
Port: 5432
#### Elastic Beanstalk
The application server is hosted on AWS Elastic Beanstalk. Elastic Beanstalk extracts and executes the application on an endpoint once it has been built, archived, and uploaded to an S3 bucket.

EB URL: `http://udagramapi-env-1.eba-wukrccbz.eu-central-1.elasticbeanstalk.com`

#### S3 Bucket
AWS S3 Bucket is used to deploy the frontend application. The packaged assets are uploaded to an S3 bucket, which is made publicly accessible.

Bucket URL: `http://udagram-frontend-01.s3-website.eu-central-1.amazonaws.com`
