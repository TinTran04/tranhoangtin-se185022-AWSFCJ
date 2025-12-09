---
title: "Worklog Tuần 11"
date: 2025-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

* Triển khai ứng dụng web thương mại điện tử lên **AWS Amplify** trên môi trường AWS thật.
* Tích hợp **Amazon Cognito** vào web để quản lý đăng nhập/người dùng.
* Thiết lập **S3** để lưu trữ hình ảnh và cấu hình web sử dụng hình ảnh từ S3.
* Chuyển data từ **Supabase** sang **EC2** và sử dụng EC2 làm nguồn dữ liệu chính.
* Hoàn thiện bước tạo và cấu hình các **dịch vụ AWS cloud** cốt lõi theo kiến trúc đã đề ra.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                                           | Ngày bắt đầu           | Ngày hoàn thành        | Nguồn tài liệu |
| --- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------- | ---------------------- | ------------- |
| 2   | - Online meeting: triển khai ứng dụng web lên **AWS Amplify** trên môi trường AWS thật <br> - Tích hợp **Cognito** vào web  <br> - Bắt đầu tạo các **AWS Cloud services** cần thiết theo kiến trúc (Amplify app, Cognito user pool, S3 bucket, EC2, …) | 01/12/2025    | 03/12/2025             |               |
| 3   | - Hoàn tất việc tích hợp **Cognito** vào web và xác nhận login hoạt động <br> - Deploy thành công web lên **Amplify** (build & hosting ổn định) <br> - Tạo S3 bucket, upload hình ảnh sản phẩm và cấu hình web đọc hình ảnh trực tiếp từ **S3**                                          | 03/12/2025             | 04/12/2025             |               |
| 4   | - Chuyển dữ liệu từ **Supabase** sang database trên **EC2** (import/export, migrate schema & data) <br> - Cấu hình lại ứng dụng web để sử dụng **EC2** làm nguồn dữ liệu chính thay cho Supabase <br> - Kiểm tra nhanh các chức năng chính sau khi đổi nguồn data                       | 04/12/2025             | 04/12/2025             |               |


### Kết quả đạt được tuần 11:

* **Web thương mại điện tử** đã được:
  * Deploy thành công lên **AWS Amplify** trên môi trường AWS thật.
  * Build & hosting ổn định, có thể truy cập và test trực tiếp trên Amplify.

* **Cognito**:
  * Đã được tích hợp vào web, hỗ trợ đăng nhập/người dùng theo đúng hướng kiến trúc AWS.
  * Luồng đăng nhập cơ bản hoạt động, sẵn sàng cho các bước mở rộng sau này (phân quyền, bảo mật,…).

* **S3 & media**:
  * Tạo S3 bucket và upload hình ảnh sản phẩm lên S3.
  * Cấu hình lại web để **sử dụng hình ảnh từ S3**, tách biệt phần media khỏi source code.

* **Data layer (Supabase → EC2)**:
  * Dữ liệu đã được **chuyển từ Supabase sang EC2**.
  * Ứng dụng web đã được cấu hình lại để sử dụng database trên EC2 làm nguồn dữ liệu chính.
  * Kiểm tra nhanh các chức năng chính sau khi đổi data cho thấy hệ thống vẫn hoạt động ổn.

* **Dịch vụ AWS cloud cốt lõi**:
  * Hoàn thành bước đầu tạo và cấu hình các dịch vụ quan trọng: Amplify, Cognito, S3, EC2, … theo đúng định hướng kiến trúc.
  * Tạo nền tảng vững chắc để các tuần sau tập trung vào phần **clickstream, ETL và analytics**.
