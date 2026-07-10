---
title: "Worklog Week 10"
date: 2026-06-23
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:
- Switch the file upload flow to S3 Upload Bucket using presigned URLs.
- Separate the Word document import feature into an AWS Lambda function for asynchronous handling.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                 | Start Date | Completion Date | Reference Material                        |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ----------------------------------------- |
| 1   | - **Backend & S3 Configuration:** <br>&emsp; + Configure S3 bucket CORS and IAM policies <br>&emsp; + Implement backend API to generate S3 presigned URLs            | 23/06/2026 | 23/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 2   | - **Frontend Integration:** <br>&emsp; + Update the frontend application to request presigned URLs and upload files directly to S3 <br>&emsp; + Verify S3 prefixes   | 24/06/2026 | 24/06/2026      | <https://docs.aws.amazon.com/AmazonS3/latest/userguide/notification-how-to-event-types-and-destinations.html>                    |
| 3   | - **Lambda Provisioning:** <br>&emsp; + Create the Word Import Lambda function <br>&emsp; + Set up the deployment package with `.docx` parsing libraries             | 25/06/2026 | 25/06/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - **Parsing & Database Logic:** <br>&emsp; + Write the Lambda logic to parse `.docx` content <br>&emsp; + Connect the Lambda to MongoDB and map question data schemas| 26/06/2026 | 26/06/2026      |<https://docs.aws.amazon.com/lambda/>         |
| 5   | - **End-to-End Testing:** <br>&emsp; + Test the complete upload and asynchronous import pipeline <br>&emsp; + Validate data integrity within MongoDB                 | 27/06/2026 | 27/06/2026      | Internal Project Docs                     |

### Week 10 Achievements:
* Successfully transitioned the main file upload flow to use S3 presigned URLs, offloading heavy file transfer traffic from the core backend.
* Verified that all uploaded files are properly categorized and saved into their correct S3 prefixes (folder structures).
* Successfully decoupled the heavy Word document processing task by moving it into a dedicated, asynchronous AWS Lambda function.
* The Word Import Lambda is fully functional: it accurately parses `.docx` files, structures the data, and successfully saves the extracted questions into the MongoDB database.