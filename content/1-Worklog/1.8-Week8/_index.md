---
title: "Week 8 Worklog"
date: 2026-06-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:
* Complete Frontend interaction for the Serverless system.
* Understand AWS security responsibilities and monitoring tools (Security Core - Week 1).
* Define the MVP scope, review the current source code, and finalize the AWS Serverless Hybrid architecture for Examora.
* Implement authentication with Cognito/SES, deploy the Express backend to Lambda, and secure APIs using API Gateway JWT Authorizer.

### Workshop Team
* The goal for the week is to define the MVP scope, review the current source code, and finalize the AWS Serverless Hybrid architecture for Examora. 
* The outcome is getting a grasp of the frontend/backend structure, deciding which modules to keep, which modules to move to AWS, and having an initial implementation backlog.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                    | Start Date | Completion Date | Reference Material                        |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ----------------------------------------- |
| 1   | - **Security Core:** Learn about the AWS Shared Responsibility Model and monitoring tools (Amazon CloudWatch & AWS CloudTrail)                                          | 06/01/2026 | 06/01/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 2   | - **Workshop Team - Code Review:** Deep dive into Examora's current frontend and backend source code to understand the existing structure and data flow                 | 06/02/2026 | 06/02/2026      | <https://docs.aws.amazon.com/apigateway/>                    |
| 3   | - **Workshop Team - Architecture:** Define the MVP scope, decide which modules remain in the current stack, and which transition to the AWS Serverless Hybrid model     | 06/03/2026 | 06/03/2026      | ExamoraServerless/01_Examora_KienTruc_Serverless.md                     |
| 4   | - **Backend Migration & Auth:** Create the initial implementation backlog. Configure Amazon Cognito/SES and deploy the refactored Express backend to AWS Lambda         | 06/04/2026 | 06/04/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - **Frontend & API Security:** Connect the frontend to the serverless APIs and secure the endpoints using an Amazon API Gateway JWT Authorizer                          | 06/05/2026 | 06/05/2026      | <https://cloudjourney.awsstudygroup.com/> |

### Week 8 Achievements:
* Gained a solid understanding of AWS security responsibilities and core monitoring services.
* Successfully audited the existing Examora frontend and backend source code to map out dependencies.
* Finalized the MVP scope and made strategic architectural decisions regarding which modules to migrate to AWS.
* Drafted a comprehensive, actionable implementation backlog for the new Serverless Hybrid architecture.
* Integrated Amazon Cognito and SES for secure, managed user authentication and communication.
* Successfully deployed the Express application to AWS Lambda and secured all API interactions using a JWT Authorizer.