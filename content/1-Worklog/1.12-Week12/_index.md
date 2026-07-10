---
title: "Worklog Week 12"
date: 2026-07-06
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Week 12 Objectives:
* **Weekly goal:** Deploy the frontend on Amplify Hosting, set up Route 53/domain, and complete testing, proposal, and workshop report.
* **Results achieved:** The frontend is running on Amplify, CORS supports local/Amplify/domain, the main flows have been retested, and the documentation has been updated according to the new architecture.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                 | Start Date | Completion Date | Reference Material                        |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ----------------------------------------- |
| 1   | - **Frontend Deployment:** <br>&emsp; + Connect the repository to AWS Amplify Hosting <br>&emsp; + Configure build settings and deploy the frontend application      | 06/07/2026 | 06/07/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 2   | - **Domain & DNS Management:** <br>&emsp; + Register/configure a custom domain using Amazon Route 53 <br>&emsp; + Attach the custom domain to the Amplify deployment | 06/07/2026 | 06/07/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - **CORS & Security Configuration:** <br>&emsp; + Update backend API CORS policies to accept requests from localhost, the Amplify default URL, and the custom domain | 07/07/2026 | 07/07/2026      | Internal Project Docs                     |
| 4   | - **System Retesting:** <br>&emsp; + Conduct end-to-end testing of all main application flows on the live production environment <br>&emsp; + Resolve any UI/API bugs| 08/07/2026 | 08/07/2026      | Internal Project Docs                     |
| 5   | - **Documentation & Reporting:** <br>&emsp; + Update system architecture diagrams to reflect the final setup <br>&emsp; + Complete the proposal and workshop report  | 09/07/2026 | 09/07/2026      | Internal Project Docs                     |

### Week 12 Achievements:
* Successfully deployed the frontend application to AWS Amplify Hosting, establishing a reliable continuous deployment pipeline.
* Configured Amazon Route 53 to manage DNS and successfully linked a custom domain to the production frontend.
* Resolved cross-origin resource sharing restrictions by properly updating the backend CORS settings to support local development, the Amplify URL, and the production domain.
* Performed comprehensive retesting of the main workflows (authentication, submissions, async grading, file uploads) in the live environment, confirming system stability.
* Finalized and polished all project documentation, including the technical proposal and the comprehensive workshop report, fully detailing the new AWS Serverless Hybrid architecture.