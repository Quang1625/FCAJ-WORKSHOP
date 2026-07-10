---
title: "Worklog Week 7"
date: 2026-06-02
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:
* Familiarize with Serverless architecture, AWS Lambda, and API Gateway.
* Deploy a basic serverless Backend.
* Grasp NoSQL database concepts (DynamoDB).
* Manage user identity and application authentication.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                 | Start Date | Completion Date | Reference Material                        |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ----------------------------------------- |
| 1   | - Learn Serverless architecture fundamentals <br> - Understand AWS Lambda execution models <br> - **Practice:** Create and test a simple "Hello World" Lambda function | 02/06/2026 | 02/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 2   | - Learn Amazon API Gateway concepts (REST APIs, HTTP APIs, Endpoints) <br> - **Practice:** Connect API Gateway to AWS Lambda to trigger the function via HTTP request  | 03/06/2026 | 03/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Learn NoSQL basics and Amazon DynamoDB: <br>&emsp; + Partition keys and Sort keys <br>&emsp; + Read/Write capacity modes <br> - **Practice:** Create a DynamoDB table| 04/06/2026 | 04/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - **Practice:** Update the Lambda function to read and write data to the DynamoDB table, completing the serverless backend                                           | 05/06/2026 | 05/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Learn Amazon Cognito for identity management <br> - **Practice:** <br>&emsp; + Create a Cognito User Pool <br>&emsp; + Secure the API Gateway using a Cognito Authorizer | 06/06/2026 | 06/06/2026      | <https://cloudjourney.awsstudygroup.com/> |

### Week 7 Achievements:
* Understood the core principles of serverless computing and event-driven architecture on AWS.
* Successfully authored and deployed an AWS Lambda function to execute backend code without provisioning or managing servers.
* Configured an Amazon API Gateway to route HTTP requests to the Lambda function, establishing a fully functional RESTful serverless API.
* Grasped NoSQL database fundamentals and provisioned an Amazon DynamoDB table for fast, flexible, and scalable data storage.
* Created an Amazon Cognito User Pool to handle user registration and sign-in.
* Successfully integrated Amazon Cognito with API Gateway to restrict API access strictly to authenticated users.