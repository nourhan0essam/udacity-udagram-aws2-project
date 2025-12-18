# Udagram – Image Filtering Application (AWS Deployment)

## Project Overview
Udagram is a full-stack image filtering application deployed on AWS.  
Users can register, log in, upload images, and process them using a backend image filtering service.

This project demonstrates deploying a full-stack application using:
- AWS Elastic Beanstalk (Backend API)
- AWS S3 (Frontend Hosting)
- AWS RDS (PostgreSQL Database)
- CircleCI (CI/CD Pipeline)

---

## Application Architecture
- **Frontend**: Angular application hosted on AWS S3
- **Backend**: Node.js (TypeScript) REST API deployed on AWS Elastic Beanstalk
- **Database**: PostgreSQL database hosted on AWS RDS
- **CI/CD**: CircleCI pipeline triggered on every push to the `main` branch

---

## Dependencies
- Node v14.15.1 (LTS) or more recent
- npm 6.14.8 (LTS) or more recent
- AWS CLI v2
- A RDS database running Postgres.
- A S3 bucket for hosting uploaded pictures.

---

## Live Application Links

- **Frontend Application (S3)**  
  👉 http://udagram-frontend-1092.s3-website-us-east-1.amazonaws.com/

- **Backend API (Elastic Beanstalk)**  
  👉 http://udacity-udagram-api-env.eba-rgr2nzr4.us-east-1.elasticbeanstalk.com/

---

## Screenshots

### Working Application
![Working App](./screenshots/app.png)

### CircleCI Successful Pipeline
![CircleCI](./screenshots/circleci.png)

### AWS RDS Database
![RDS](./screenshots/rds1.png)

### AWS Elastic Beanstalk Backend
![Elastic Beanstalk](./screenshots/elastic.png)

### AWS S3 Frontend Hosting
![S3](./screenshots/s3.png)

---

## CI/CD Pipeline
- Code is pushed to GitHub
- CircleCI pipeline runs automatically
- Build, test, and deployment steps are executed
- Secrets are managed using CircleCI Environment Variables

---

## Environment Variables
All sensitive values (AWS keys, DB credentials, JWT secret) are:
- **NOT** stored in source code
- Configured securely in CircleCI and Elastic Beanstalk

---

## Author
Nourhan Essam