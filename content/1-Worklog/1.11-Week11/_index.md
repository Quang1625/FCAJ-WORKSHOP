---
title: "Worklog Week 11"
date: 2026-06-22
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:
- **Weekly goal:** Separate the grading logic from the submission request using SQS Grading Queue and Lambda Grading Worker.  
- **Result achieved:** Backend saves the submission with a grading status, sends a job to SQS, and the worker handles grading/updating the results in MongoDB.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                 | Start Date | Completion Date | Reference Material                        |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ----------------------------------------- |
| 1   | - **Queue Provisioning:** <br>&emsp; + Create the SQS Grading Queue <br>&emsp; + Configure Dead-Letter Queue (DLQ) for failed grading jobs                           | 06/22/2026 | 06/22/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 2   | - **Backend Refactoring:** <br>&emsp; + Update the Express API to save initial submissions with a 'grading' status <br>&emsp; + Integrate AWS SDK to push jobs to SQS| 06/23/2026 | 06/23/2026      | Internal Project Docs                     |
| 3   | - **Lambda Setup:** <br>&emsp; + Provision the Lambda Grading Worker <br>&emsp; + Configure IAM roles for SQS read access and MongoDB write access                   | 06/24/2026 | 06/24/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - **Grading Logic Implementation:** <br>&emsp; + Write Lambda logic to process SQS messages and calculate scores <br>&emsp; + Connect Lambda to MongoDB to update results| 06/25/2026 | 06/25/2026      | Internal Project Docs                     |
| 5   | - **End-to-End Testing:** <br>&emsp; + Test the asynchronous submission flow from the frontend to the database <br>&emsp; + Verify SQS message processing and deletion| 06/26/2026 | 06/26/2026      | Internal Project Docs                     |

### Week 11 Achievements:
* Successfully decoupled the heavy exam grading logic from the immediate user submission flow using Amazon SQS.
* Improved API response times by having the backend instantly return a success response while saving a temporary "grading" status to the database.
* Provisioned and securely configured an SQS Grading Queue to buffer submission jobs, ensuring no data is lost during traffic spikes.
* Developed and deployed a dedicated Lambda Grading Worker that automatically scales to process messages from the queue.
* Verified that the Lambda worker accurately calculates scores and successfully updates the final grading results directly into MongoDB.