---
title: "Worklog Week 9"
date: 2026-06-08
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:
- Migrate the file upload flow to S3 Upload Bucket using presigned URLs and separate the Word import feature into an asynchronous Lambda function.
- Decouple grading logic from the exam submission request using SQS Grading Queue and Lambda Grading Worker.  
- Decouple PDF generation logic from the exam submission request using SQS PDF Generation Queue and Lambda PDF Generation Worker.  
- Decouple email notification logic from the exam submission request using SQS Email Notification Queue and Lambda Email Notification Worker.

### Workshop Team
- **Weekly goal:** Implement authentication with Cognito/SES, deploy the Express backend to Lambda, and protect the API using API Gateway JWT Authorizer.
- **Results achieved:** Completed the registration flow, email OTP, login, MongoDB profile sync, Lambda Backend API, and basic API Gateway testing.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                    | Start Date | Completion Date | Reference Material                        |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ----------------------------------------- |
| 1   | - **Workshop Team - Auth Flow:** Implement user registration, email OTP using Amazon SES, and login flow using Amazon Cognito <br>&emsp; + Sync user profiles with MongoDB | 06/08/2026 | 06/08/2026      | <https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api.html/>                |
| 2   | - **Workshop Team - Backend & API:** Deploy the Express backend to AWS Lambda <br>&emsp; + Configure API Gateway JWT Authorizer and conduct basic endpoint testing       | 06/09/2026 | 06/09/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - **File Uploads & Import:** Migrate file upload flow to S3 using presigned URLs <br>&emsp; + Extract and refactor the Word import feature into an async Lambda function | 06/10/2026 | 06/10/2026      | <https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-jwt-authorizer.html/>                  |
| 4   | - **Grading & PDF Decoupling:** Provision SQS Queues for Grading and PDF Generation <br>&emsp; + Develop and attach Lambda Workers to process these respective queues    | 06/11/2026 | 06/11/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - **Email Decoupling:** Provision the SQS Email Notification Queue <br>&emsp; + Develop the Lambda Email Notification Worker and test the fully decoupled submission flow| 06/12/2026 | 06/12/2026      | <https://cloudjourney.awsstudygroup.com/> |

### Week 9 Achievements:
* Successfully completed the user authentication workflow, including registration, email OTP verification via SES, and login via Cognito.
* Established seamless data synchronization between the authentication layer and user profiles stored in MongoDB.
* Deployed the Express backend as a serverless API on AWS Lambda and successfully protected the endpoints using an API Gateway JWT Authorizer.
* Optimized application performance by migrating direct file uploads to S3 via presigned URLs and moving heavy Word imports to a background Lambda function.
* Architected a highly decoupled exam submission system using Amazon SQS to handle grading, PDF generation, and email notifications asynchronously.
* Developed and deployed dedicated Lambda Workers for each SQS queue, ensuring the core API remains fast and non-blocking for end users.