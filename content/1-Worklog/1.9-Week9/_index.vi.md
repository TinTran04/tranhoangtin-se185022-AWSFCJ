---
title: "Worklog Tuần 9"
date: 2025-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:

* Rà soát lại hướng triển khai **CloudFront, Amplify** và thống nhất cách sử dụng **LocalStack**.
* Điều chỉnh **kiến trúc hệ thống** cho phù hợp với thiết kế mới (Amplify, Supabase/PostgreSQL, LocalStack,…).
* Tiếp tục hoàn thiện **giao diện web (UI)** và xử lý các lỗi còn tồn tại.
* Bắt đầu làm quen với **Docker** để đóng gói môi trường phát triển.
* Chuẩn bị **template báo cáo (docx)** và định hình cách đưa nội dung lên Hugo.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                                                                                | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ------------- |
| 2   | - Cá nhân: sửa lại **UI web** theo feedback của team (layout, màu sắc, lỗi hiển thị) <br> - Tiếp tục tìm hiểu về **S3, Cognito, CloudFront, Amplify, LocalStack** để nắm rõ hơn vai trò của từng dịch vụ trong kiến trúc <br> - Kiểm tra lại web sau khi sửa UI để đảm bảo không phát sinh lỗi mới | 03/11/2025   | 06/11/2025      |               |
| 3   | - Họp nhóm: xem lại phương án dùng **CloudFront & Amplify** trong kiến trúc <br> - Thống nhất sử dụng **LocalStack bản Base** để mô phỏng nhiều dịch vụ (đặc biệt là Cognito) <br> - Chỉnh lại luồng kiến trúc tương ứng với việc dùng **Supabase/PostgreSQL** làm database cho web          | 09/11/2025   | 10/11/2025      |               |             |
| 4   | - Họp: tìm hiểu cách sử dụng **Docker** (image, container, cài thư viện vào image) <br> - Đề xuất ý tưởng dùng **Docker + LocalStack** làm môi trường phát triển chuẩn cho cả nhóm                                     | 11/11/2025   | 11/11/2025      |               |
| 5   | - Họp nhóm: chỉnh sửa và chốt **architecture diagram v9** <br> - Cá nhân: hoàn thiện file **docx template** (các phần worklog, workshop, mô tả kiến trúc) <br> - Chia nhỏ các phần nội dung, phân công người phụ trách và đặt deadline rõ ràng cho từng phần | 12/11/2025   | 13/11/2025      |               |


### Kết quả đạt được tuần 9:

* **Giao diện web (UI)** đã được rà soát và cải thiện:
  * Sửa một số lỗi hiển thị, căn lề, màu sắc theo góp ý của team.
  * Web ổn định hơn trên local, sẵn sàng cho việc tích hợp thêm các dịch vụ AWS.

* Nhóm đã **hiểu rõ hơn vai trò các dịch vụ AWS** trong kiến trúc:
  * Tiếp tục tìm hiểu và thống nhất cách dùng **S3, Cognito, CloudFront, Amplify, LocalStack**.
  * Quyết định chọn **LocalStack bản Base** để giả lập nhiều dịch vụ (đặc biệt là Cognito) trong môi trường dev.
  * Chốt hướng dùng **Supabase/PostgreSQL** làm database cho web.

* Kiến trúc hệ thống được cập nhật lên **phiên bản v9**:
  * Điều chỉnh lại luồng dữ liệu phù hợp với Amplify, Supabase và LocalStack.
  * Danh sách các service chính trong mô hình đã được thống nhất, giúp nhóm có “khung” rõ ràng để triển khai.

* Bước đầu **làm quen với Docker**:
  * Nắm được khái niệm image, container và cách cài thư viện vào image.
  * Đặt nền tảng cho việc dùng **Docker + LocalStack** làm môi trường phát triển chuẩn cho cả nhóm.

* **Template báo cáo (docx)** đã có bản phác thảo và phân chia công việc:
  * Hoàn thiện khung cho các phần: worklog, workshop, mô tả kiến trúc.
  * Chia nhỏ nội dung, phân công người phụ trách và đặt deadline rõ ràng, giúp việc viết báo cáo sau này dễ dàng và nhất quán hơn.

