---
title: "Worklog Tuần 10"
date: 2025-01-01
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Mục tiêu tuần 10:

* Kiểm tra lại **template báo cáo (docx)** và rà soát cấu trúc nội dung.
* Chạy và nghiên cứu lại **dự án web thương mại điện tử**, kiểm tra độ ổn định.
* Làm quen và thực hành với **Docker** và **LocalStack**.
* Deploy web lên **Vercel**, xử lý các lỗi build, chuẩn bị bước chuyển từ **Clerk** sang **Cognito**.
* Hoàn tất bước chuẩn bị cho môi trường **LocalStack Pro + Terraform + Amplify + Cognito + PostgreSQL trên EC2 + S3** theo kiến trúc đề ra.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                                                                                                                                                           | Ngày bắt đầu           | Ngày hoàn thành        | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------- | ---------------------- | ------------- |
| 2   | - Kiểm tra lại **template docx** (bố cục, mục lục, phần worklog/workshop) <br> - Chạy lại và nghiên cứu cấu trúc dự án web thương mại điện tử <br> - Kiểm tra website bán hàng đã ổn định chưa (load trang, điều hướng, tương tác cơ bản) <br> - Bắt đầu làm quen với **LocalStack** <br> - Kích hoạt **GitHub Student** <br> - Học cách sử dụng **Docker + LocalStack** ở mức cơ bản | 21/11/2025   | 21/11/2025     |               |
| 3   | - Test web sàn thương mại điện tử: <br>&emsp; + Kiểm tra các chức năng cơ bản (xem thông tin, thêm giỏ, tiến hành mua,…) <br> - Thử dùng **Clerk** để đăng nhập, lấy user id về database nhưng không phù hợp yêu cầu → thống nhất **chuyển sang Cognito** <br> - Deploy web lên **Vercel**: fix nhiều lỗi build (next.config.ts, package.json, ESLint, env) cho đến khi deploy thành công, lưu được user id vào database (user pool) | 23/11/2025    | 24/11/2025     |               |
| 4   | - Họp online: học và thực hành **LocalStack Pro**  <br>&emsp; + Cấu hình API Key cho LocalStack Pro <br>&emsp; + Chạy docker image LocalStack <br>&emsp; + Apply **Terraform** vào LocalStack theo đúng kiến trúc <br> - Terraform: chỉnh sửa file TF cho khớp với diagram, kích hoạt CloudFront trong Amplify <br> - Amplify: nghiên cứu cách đưa project **NextJS** vào Amplify <br> - Cognito: thử nghiệm implement Cognito trong môi trường Amplify local <br> - Web data: chuẩn bị kế hoạch deploy **PostgreSQL lên EC2 (subnet 1)** và đẩy file ảnh mẫu lên **S3** | 24/11/2025    | 24/11/2025    |               |


### Kết quả đạt được tuần 10:

* **Template báo cáo (docx)**:
  * Đã được kiểm tra lại về bố cục và nội dung chính (worklog, workshop, mô tả dự án).
  * Giúp nhóm có một khung tài liệu rõ ràng hơn để sử dụng cho các tuần sau.

* **Dự án web thương mại điện tử**:
  * Đã chạy lại và kiểm tra độ ổn định, các chức năng cơ bản hoạt động đúng (xem sản phẩm, thêm vào giỏ, tiến hành mua,…).
  * Từ việc thử dùng **Clerk** và nhận ra không phù hợp, nhóm thống nhất **chuyển sang Cognito** để đồng bộ với kiến trúc AWS.

* **Deploy web lên Vercel**:
  * Gặp nhiều lỗi build (next.config.ts, package.json, trùng file cấu hình, lỗi ESLint, env) nhưng đã xử lý lần lượt.
  * Sau 4 lần thất bại, lần thứ 5 deploy **thành công**, web chạy ổn định trên Vercel và lưu được user id vào database thông qua user pool.

* **Docker & LocalStack Pro**:
  * Các thành viên đã làm quen với **Docker** (image, container, cách cài thư viện vào image).
  * Cấu hình thành công **LocalStack Pro**: set API key, chạy được docker image, apply Terraform vào LocalStack.
  * Đây là bước quan trọng để chuẩn hóa môi trường dev cho toàn nhóm.

* **Hạ tầng theo kiến trúc mục tiêu**:
  * Terraform được chỉnh sửa để khớp với sơ đồ kiến trúc và kích hoạt **CloudFront trong Amplify**.
  * Đã bắt đầu nghiên cứu cách đưa **NextJS** vào Amplify, implement Cognito trong môi trường Amplify local.
  * Chuẩn bị kế hoạch cho phần web data: **PostgreSQL trên EC2 (subnet 1)** và upload file ảnh lên **S3**, làm nền tảng cho các tuần triển khai tiếp theo.
