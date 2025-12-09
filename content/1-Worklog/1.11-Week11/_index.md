---
title: "Worklog Week 11"
date: 2025-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Deploy the e-commerce web application to **AWS Amplify** in the real AWS environment.
* Integrate **Amazon Cognito** into the web app to manage logins/users.
* Set up **S3** for image storage and configure the web app to use images from S3.
* Migrate data from **Supabase** to **EC2** and use EC2 as the main data source.
* Complete the creation and configuration of the core **AWS cloud services** according to the planned architecture.

### Tasks to be carried out this week:

| Day | Tasks                                                                                                                                                                                                                                           | Start date  | Completion date | References |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------- | ---------------- | ---------- |
| 2   | - Online meeting: deploy the web application to **AWS Amplify** in the real AWS environment <br> - Integrate **Cognito** into the web app  <br> - Start creating the required **AWS Cloud services** according to the architecture (Amplify app, Cognito user pool, S3 bucket, EC2, …) | 01/12/2025  | 03/12/2025       |            |
| 3   | - Complete **Cognito** integration into the web app and verify that login works <br> - Successfully deploy the web app to **Amplify** (stable build & hosting) <br> - Create an S3 bucket, upload product images, and configure the web app to load images directly from **S3**        | 03/12/2025  | 04/12/2025       |            |
| 4   | - Migrate data from **Supabase** to the database on **EC2** (import/export, migrate schema & data) <br> - Reconfigure the web application to use **EC2** as the main data source instead of Supabase <br> - Quickly test core features after switching the data source                 | 04/12/2025  | 04/12/2025       |            |


### Week 11 Achievements:

* **E-commerce web application**:
  * Successfully deployed to **AWS Amplify** in the real AWS environment.
  * Build & hosting are stable; the app can be accessed and tested directly on Amplify.

* **Cognito**:
  * Integrated into the web app to support user login/management in line with the AWS architecture.
  * The basic login flow works and is ready for future enhancements (authorization, security, …).

* **S3 & media**:
  * Created an S3 bucket and uploaded product images to S3.
  * Reconfigured the web app to **use images from S3**, separating media from the source code.

* **Data layer (Supabase → EC2)**:
  * Data has been **migrated from Supabase to EC2**.
  * The web application has been reconfigured to use the EC2-hosted database as the main data source.
  * Quick checks of core features after switching data show that the system still operates correctly.

* **Core AWS cloud services**:
  * Completed the initial creation and configuration of key services: Amplify, Cognito, S3, EC2, … according to the architectural direction.
  * Established a solid foundation so that the following weeks can focus on **clickstream, ETL, and analytics**.
