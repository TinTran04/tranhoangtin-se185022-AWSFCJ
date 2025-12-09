---
title: "Worklog Week 9"
date: 2025-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives

* Review the approach for **CloudFront, Amplify** and agree on how to use **LocalStack**.
* Adjust the **system architecture** to match the new design (Amplify, Supabase/PostgreSQL, LocalStack, …).
* Continue improving the **web UI** and fixing remaining issues.
* Start getting familiar with **Docker** to containerize the development environment.
* Prepare the **report template (docx)** and plan how to publish content on Hugo.

### Tasks for this week

| Day | Task                                                                                                                                                                                                                                                                                | Start Date  | End Date    | References |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | ----------- | ---------- |
| 2   | - Individual: fix the **web UI** based on team feedback (layout, colors, display issues) <br> - Continue learning about **S3, Cognito, CloudFront, Amplify, LocalStack** to better understand the role of each service in the architecture <br> - Re-test the web after UI changes to ensure no new bugs are introduced | 03/11/2025  | 06/11/2025  |            |
| 3   | - Team meeting: review the approach of using **CloudFront & Amplify** in the architecture <br> - Agree to use **LocalStack Base** to emulate multiple AWS services (especially Cognito) <br> - Update the architecture flow to reflect using **Supabase/PostgreSQL** as the web database | 09/11/2025  | 10/11/2025  |            |
| 4   | - Meeting: explore how to use **Docker** (image, container, installing libraries into the image) <br> - Propose the idea of using **Docker + LocalStack** as the standard development environment for the whole team                                                               | 11/11/2025  | 11/11/2025  |            |
| 5   | - Team meeting: update and finalize **architecture diagram v9** <br> - Individual: complete the **docx template** (worklog, workshop, architecture description sections) <br> - Break down the content, assign owners, and set clear deadlines for each part                      | 12/11/2025  | 13/11/2025  |            |


### Week 9 Outcomes

* The **web UI** has been reviewed and improved:
  * Fixed several display, alignment, and color issues based on team feedback.
  * The web app runs more stably on local, ready for further AWS service integration.

* The team **understands the roles of AWS services** in the architecture more clearly:
  * Continued to study and align on how to use **S3, Cognito, CloudFront, Amplify, LocalStack**.
  * Decided to use **LocalStack Base** to emulate multiple AWS services (especially Cognito) in the dev environment.
  * Confirmed **Supabase/PostgreSQL** as the database solution for the web app.

* The system architecture has been updated to **version 9**:
  * Data flows were adjusted to better match Amplify, Supabase, and LocalStack.
  * The list of core services in the model has been finalized, giving the team a clear “frame” to implement.

* First steps in working with **Docker**:
  * Understood the concepts of image, container, and how to install libraries into an image.
  * Laid the groundwork for using **Docker + LocalStack** as a standard development environment for the team.

* The **report template (docx)** now has an initial draft and task breakdown:
  * A structure has been defined for the worklog, workshop, and architecture description sections.
  * Content has been split into smaller parts with assigned owners and clear deadlines, making future reporting easier and more consistent, and smoother to publish on Hugo.
