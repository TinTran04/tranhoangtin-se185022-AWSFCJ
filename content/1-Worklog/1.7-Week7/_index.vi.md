---
title: "Worklog Tuần 7"
date: 2025-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Nắm **tổng quan dự án Batch-based Clickstream Analytics & sessionization**.
* Xác định **mục tiêu, vấn đề cần giải quyết và phương pháp tiếp cận** của dự án.
* Tìm hiểu **các dịch vụ AWS** phù hợp cho kiến trúc clickstream.
* Phác thảo **kiến trúc hệ thống** và ước tính **chi phí triển khai** cơ bản.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                                                                                                         | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                           |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------------------------------------------------------------------------------------------------- |
| 2   | - Họp online kick-off với các thành viên trong nhóm FCJ <br> - Giới thiệu tổng quan dự án: sessionization & clickstream cho website thương mại điện tử <br> - Thống nhất phạm vi, mục tiêu, sản phẩm cuối (web + pipeline phân tích)                                                                            | 20/10/2025   | 20/10/2025      |                                                                         |
| 3   | - Tìm hiểu lý thuyết về **clickstream** và **sessionization**: khái niệm, ý nghĩa, các chỉ số thường dùng <br> - Tham khảo một số kiến trúc tham chiếu clickstream trên AWS <br> - Ghi lại yêu cầu chức năng & phi chức năng liên quan đến dữ liệu, bảo mật, hiệu năng                                      | 21/10/2025   | 21/10/2025      |                                |
| 4   | - Họp online cả nhóm để liệt kê những **dịch vụ AWS** có thể sử dụng trong dự án: Amplify, CloudFront, S3, API Gateway, Lambda, EventBridge, EC2, RDS/EC2 DW, Cognito, IAM, CloudWatch, SNS,… <br> - Phân tích vai trò từng dịch vụ trong kiến trúc (frontend, ingest, storage, ETL, analytics, monitoring) | 22/10/2025   | 22/10/2025      |                    |
| 5   | - Bắt đầu **thiết kế kiến trúc tổng thể**: <br>&emsp; + Vẽ luồng dữ liệu  <br> - Cả nhóm review sơ bộ kiến trúc qua cuộc họp online                 | 23/10/2025   | 23/10/2025      |                                      |
| 6   | - Hoàn thiện bản **architecture diagram phiên bản 1**   | 24/10/2025   | 24/10/2025      |                                                   |


### Kết quả đạt được tuần 7:

* Cả nhóm đã **hiểu rõ tổng quan dự án**:  
  * Bài toán thu thập & phân tích dữ liệu clickstream cho website  bán máy tính & thiết bị điện tử.  
  * Nhu cầu **sessionization** để nhóm các hành vi của người dùng theo phiên truy cập.

* Xác định được **mục tiêu & vấn đề cần giải quyết**:
  * Xây dựng pipeline batch-based clickstream từ frontend → lưu trữ → ETL → phân tích.  
  * Tận dụng các dịch vụ managed của AWS để giảm chi phí vận hành và tăng khả năng mở rộng.

* Đã có **bản vẽ kiến trúc phiên bản 1** cho toàn hệ thống và thống nhất trong nhóm qua các buổi họp online.