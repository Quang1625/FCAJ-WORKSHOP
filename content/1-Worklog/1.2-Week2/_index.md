---
title: "Worklog Week 2"
date: 2026-04-20
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---



###  Week 2 Objectives

* **Complete tasks on the AWS Console**: Collect a total of **$200 USD in AWS Credits** to optimize costs during hands-on practice with paid services.
* **Overview the AWS service ecosystem**: Explore core service groups (*Compute, Storage, Networking, Database*, etc.), system architecture, and AWS pricing models to prepare for designing and deploying optimal and cost-effective infrastructure in the future.

---

###  Tasks to Deploy This Week

| Day | Task | Start Date | Completion Date | Reference Material |
| :---: | :--- | :---: | :---: | :--- |

| **Tue** | - Get familiar with the AWS Management Console interface <br> - Install and configure AWS CLI on the personal computer (*Access Key, Secret Key, Default Region*) <br> - Hands-on: Execute basic AWS CLI commands to check resources | 21/04/2026 | 21/04/2026 | [AWS Cloud Journey](https://cloudjourney.awsstudygroup.com/) |
| **Wed** | - Grasp basic Amazon EC2 services: *Instance categories, AMI (Amazon Machine Image), EBS (Elastic Block Store), Elastic IP* <br> - Learn about security methods and SSH connection from a workstation to EC2 | 22/04/2026 | 22/04/2026 | [AWS Cloud Journey](https://cloudjourney.awsstudygroup.com/) |
| **Thu** | - **Practical Technical Lab Deployment**: <br>&emsp; + Provision a complete EC2 instance in practice <br>&emsp; + Create and attach an additional EBS volume <br>&emsp; + Connect via SSH and manage resources concurrently via Console & CLI | 23/04/2026 | 23/04/2026 | [AWS Cloud Journey](https://cloudjourney.awsstudygroup.com/) |

---

###  Week 2 Achievements

| Day | Task | Detailed Achievement | Proof / Image |
| :---: | :--- | :--- | :---: |
| **Tue** | **Communication Methods & CLI Setup** | Completed **Module 1 (Part 2: Interacting with AWS)**: <br> Learned 3 main ways to control the AWS system: <br> - **AWS Management Console**: Intuitive web interface. Clearly distinguished the difference between the *Root User* (used only when absolutely necessary, strictly protected with MFA) and the *IAM User* (an account with flexibly assigned permissions for daily tasks). <br> - **AWS CLI**: Command-line tool for quick operations and automation scripting. Safely configured on the local machine (strictly do not publicize Access/Secret Keys on GitHub). <br> - **AWS SDK**: Library suites (Python, Java, etc.) for developers to integrate API calls directly into source code. | *(CLI configuration terminal illustration)* |
| **Wed** | **EC2 Service Architecture** | Equipped with a solid theoretical foundation on *Instance families*, *AMI structures*, *EBS storage*, *IP routing methods*, and security practices via *SSH Key Pairs*. | *(EC2 Console control interface image)* |
| **Thu** | **Practical Lab Operations** | Successfully deployed an EC2 virtual server, integrated an additional EBS drive, and maintained a stable SSH connection from the personal computer; became proficient in cross-managing resources between the Web interface and the command line. | *(Successful SSH connection to EC2 illustration)* |

