---
title: "Worklog Week 7"
date: 2025-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives

* Understand the **overall scope of the Batch-based Clickstream Analytics & Sessionization project**.
* Identify the **project objectives, problem statement, and approach**.
* Explore **AWS services** suitable for the clickstream analytics architecture.
* Draft the **system architecture** and perform a rough **cost estimation**.

### Tasks for this week

| Day | Task                                                                                                                                                                                                                                                                                                                         | Start Date | End Date   | References |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | ---------- |
| Mon | - Online kick-off meeting with FCJ team members. <br> - Present an overview of the project: sessionization & clickstream for an e-commerce website. <br> - Align on scope, objectives and final deliverables (web application + analytics pipeline).                                                                         | 20/10/2025 | 20/10/2025 |            |
| Tue | - Study the theory of **clickstream** and **sessionization**: concepts, importance and common metrics. <br> - Review several reference architectures for clickstream analytics on AWS. <br> - Note down functional and non-functional requirements related to data, security and performance.                                 | 21/10/2025 | 21/10/2025 |            |
| Wed | - Online team discussion to list **AWS services** that can be used in the project: Amplify, CloudFront, S3, API Gateway, Lambda, EventBridge, EC2, RDS/EC2 DW, Cognito, IAM, CloudWatch, SNS, … <br> - Analyze the role of each service in the architecture (frontend, ingest, storage, ETL, analytics, monitoring).          | 22/10/2025 | 22/10/2025 |            |
| Thu | - Start **designing the overall architecture**: <br>&emsp; + Draw the main data flows through the system. <br> - Conduct an online review meeting to get initial feedback on the architecture from all team members.                                                                  | 23/10/2025 | 23/10/2025 |            |
| Fri | - Finalize **Architecture Diagram – Version 1** for the project based on team feedback.                                                                                                                                                                                                                                      | 24/10/2025 | 24/10/2025 |            |

### Outcomes of Week 7

* The whole team has a **clear understanding of the project**:  
  * The problem of collecting and analyzing clickstream data for an e-commerce website selling laptops & electronic devices.  
  * The need for **sessionization** to group user behaviors into meaningful sessions.

* Clearly defined **objectives and problems to solve**:
  * Build a batch-based clickstream pipeline from frontend → storage → ETL → analytics.  
  * Leverage managed AWS services to reduce operational overhead and improve scalability.

* Completed **Architecture Diagram – Version 1** for the entire system and reached consensus within the team through multiple online discussions.
