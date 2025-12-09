---
title: "Worklog Week 10"
date: 2025-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Week 10 Objectives:

* Review the **report template (docx)** and check the content structure.
* Run and re-examine the **e-commerce web project**, verify its stability.
* Get familiar with and practice using **Docker** and **LocalStack**.
* Deploy the web app to **Vercel**, fix build errors, and prepare for the migration from **Clerk** to **Cognito**.
* Complete preparation steps for the environment **LocalStack Pro + Terraform + Amplify + Cognito + PostgreSQL on EC2 + S3** according to the proposed architecture.

### Tasks to be carried out this week:

| Day | Tasks                                                                                                                                                                                                                                                                                                                                                               | Start date            | Completion date       | References |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- | --------------------- | ---------- |
| 2   | - Review the **docx template** (layout, table of contents, worklog/workshop sections) <br> - Rerun and study the structure of the e-commerce web project <br> - Check whether the e-commerce site is stable (page loading, navigation, basic interactions) <br> - Start getting familiar with **LocalStack** <br> - Activate **GitHub Student** <br> - Learn how to use **Docker + LocalStack** at a basic level | 21/11/2025           | 21/11/2025           |            |
| 3   | - Test the e-commerce website: <br>&emsp; + Check basic features (view details, add to cart, proceed to checkout,…) <br> - Try using **Clerk** for login and fetching user id to the database, but this does not meet the requirements → agree to **switch to Cognito** <br> - Deploy the web app to **Vercel**: fix multiple build errors (next.config.ts, package.json, ESLint, env) until deployment succeeds, and ensure user id is saved to the database (user pool) | 23/11/2025           | 24/11/2025           |            |
| 4   | - Online meeting: learn and practice **LocalStack Pro**  <br>&emsp; + Configure API Key for LocalStack Pro <br>&emsp; + Run the LocalStack docker image <br>&emsp; + Apply **Terraform** to LocalStack according to the architecture <br> - Terraform: adjust TF files to match the diagram, enable CloudFront in Amplify <br> - Amplify: research how to bring the **NextJS** project into Amplify <br> - Cognito: experiment with implementing Cognito in the Amplify local environment <br> - Web data: prepare a plan to deploy **PostgreSQL on EC2 (subnet 1)** and upload sample image files to **S3** | 24/11/2025           | 24/11/2025           |            |


### Week 10 Achievements:

* **Report template (docx)**:
  * Reviewed layout and main content sections (worklog, workshop, project description).
  * Helps the team have a clearer document framework to use for the following weeks.

* **E-commerce web project**:
  * Reran and checked stability; core features work correctly (view products, add to cart, proceed to checkout,…).
  * After trying **Clerk** and realizing it was not suitable, the team agreed to **switch to Cognito** to align with the AWS architecture.

* **Deploying the web app to Vercel**:
  * Encountered many build errors (next.config.ts, package.json, duplicated config files, ESLint, env issues) but resolved them step by step.
  * After 4 failed attempts, the 5th deployment was **successful**; the site runs stably on Vercel and can save user id to the database via the user pool.

* **Docker & LocalStack Pro**:
  * Team members became familiar with **Docker** (images, containers, how to install libraries into images).
  * Successfully configured **LocalStack Pro**: set API key, ran the docker image, and applied Terraform to LocalStack.
  * This is an important step to standardize the dev environment for the whole team.

* **Infrastructure according to the target architecture**:
  * Terraform files were adjusted to match the architecture diagram and **CloudFront in Amplify** was enabled.
  * Started researching how to bring **NextJS** into Amplify and how to implement Cognito in the Amplify local environment.
  * Prepared a plan for the web data layer: **PostgreSQL on EC2 (subnet 1)** and uploading image files to **S3**, as a foundation for the upcoming implementation weeks.
