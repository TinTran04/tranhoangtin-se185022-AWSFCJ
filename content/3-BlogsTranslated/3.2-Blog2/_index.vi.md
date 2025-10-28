---
title: "Blog 2"
date: 2025-05-09
weight: 2
chapter: false
pre: " <b> 3.2. </b> "
---



# Cách Salesforce Business Technology sử dụng AWS Direct Connect SiteLink để kết nối toàn cầu đáng tin cậy

*Bởi Alexandra Huides và Corey Harris Jr — ngày 09 tháng 5 năm 2025*

> *Lưu ý: Bài đăng này được xuất bản với sự hợp tác của Georgi Stoev, Kiến trúc sư kỹ thuật cấp cao tại Salesforce và Ravi Patel, Giám đốc kỹ thuật cấp cao tại Salesforce.*

---

## Giới thiệu

Trong bài đăng này, chúng tôi xem xét cách **Salesforce Business Technology** sử dụng **AWS Direct Connect SiteLink** để xây dựng kiến trúc kết hợp linh hoạt, tạo điều kiện mở rộng toàn cầu và tăng tốc quá trình di chuyển lên **AWS Cloud**.  
Bài viết cũng mô tả cách **SiteLink** giúp **Salesforce** thống nhất kiến trúc mạng trên **bảy địa điểm toàn cầu**, hiện đại hóa giao tiếp mạng để **giảm chi phí**, **hợp lý hóa vận hành**, và **nâng cao hiệu suất**.

---

## Tổng quan

**Salesforce** là Đối tác của **AWS** và là công ty hàng đầu thế giới trong lĩnh vực **Customer Relationship Management (CRM)**.  
Nhóm **Business Technology** của Salesforce cung cấp các dịch vụ hỗ trợ xây dựng, vận hành và chuyển đổi ứng dụng doanh nghiệp, bao gồm tài chính, bảo mật, trung tâm cuộc gọi, và kho dữ liệu công ty.

Để đáp ứng nhu cầu hoạt động toàn cầu, Salesforce cần một **kiến trúc mạng linh hoạt, có khả năng mở rộng và đảm bảo dự phòng cao**.  
Các giải pháp mạng truyền thống dựa vào Internet công cộng thường không đáp ứng được yêu cầu nghiêm ngặt về hiệu suất và độ tin cậy.  
**AWS Direct Connect SiteLink** giúp giải quyết các thách thức này bằng cách cung cấp **kết nối riêng tư, chuyên dụng**, bỏ qua Internet công cộng — đảm bảo **độ trễ thấp**, **bảo mật cao hơn**, và **khả năng phục hồi tích hợp**.

---

## AWS Direct Connect SiteLink

**AWS Direct Connect** cho phép kết nối mạng tại chỗ với **AWS** thông qua các đường truyền chuyên dụng, giúp **tối ưu độ trễ và đảm bảo hiệu suất ổn định**.  
**SiteLink** là tính năng mở rộng của Direct Connect, cho phép **kết nối trực tiếp giữa các mạng tại chỗ** qua **AWS Global Network Backbone**, mà không cần lưu lượng phải đi qua vùng (Region) AWS.

Bạn có thể:
- Truyền dữ liệu trực tiếp giữa các **Direct Connect locations** qua tuyến đường ngắn nhất  
- Tận dụng hơn **100 địa điểm Direct Connect** trên toàn thế giới  
- Kích hoạt **SiteLink** mà không cần kết nối mới – chỉ cần bật trong các **Virtual Interface (VIF)** gắn với **Direct Connect Gateway (DXGW)**

Dữ liệu sẽ di chuyển theo tuyến ngắn nhất và an toàn nhất trong mạng AWS, đảm bảo **tốc độ, độ tin cậy và bảo mật cao**.

---

## Dấu ấn toàn cầu của Salesforce Business Technology

**Salesforce Business Technology** vận hành một hạ tầng mạng trải dài trên **bảy địa điểm chiến lược**:  
- 3 tại Hoa Kỳ  
- 3 tại khu vực Châu Á – Thái Bình Dương  
- 1 tại Châu Âu  

Trước đây, Salesforce sử dụng **đường trục riêng (MPLS-based private backbone)** để kết nối các trung tâm dữ liệu.  
Tuy nhiên, mô hình này gặp phải các vấn đề:  
- Cơ sở hạ tầng tĩnh, khó mở rộng linh hoạt  
- Chi phí cao và khó quản lý nhiều nhà cung cấp dịch vụ  
- Gián đoạn kết nối kéo dài ở một số khu vực  
- Phức tạp trong việc định tuyến Layer 3 VPN  

Để khắc phục, Salesforce quyết định **hiện đại hóa toàn bộ kiến trúc mạng** bằng cách chuyển sang **AWS Direct Connect SiteLink**, giúp hệ thống **linh hoạt và mở rộng theo nhu cầu**.

![Hình 1. Mẫu kết nối trung tâm dữ liệu riêng toàn cầu sử dụng các mạch riêng.](/images/3-BlogImage/blog2-1.png)
> *Hình 1. Mẫu kết nối trung tâm dữ liệu riêng toàn cầu sử dụng các mạch riêng.*
>

---

## Giải pháp SiteLink

Salesforce triển khai **SiteLink** trên các kết nối Direct Connect hiện có bằng cách tạo **VIF chuyên dụng** cho môi trường **Production** và **Development**.  
Giải pháp này hỗ trợ nhiều luồng dữ liệu khác nhau như **Data Center–to–Data Center (DC–DC)** và **DC–AWS**, cho phép **tận dụng các kết nối sẵn có** mà không ảnh hưởng đến lưu lượng sản xuất.

Nhờ đó, Salesforce có thể duy trì **phân vùng toàn cầu**, **đảm bảo tuân thủ yêu cầu lưu trữ dữ liệu**, và đồng thời **tăng khả năng mở rộng linh hoạt**.

![Hình 2. Mẫu triển khai SiteLink toàn cầu cho môi trường Production và Development.](/images/3-BlogImage/blog2-2.png)
> *Hình 2. Mẫu triển khai SiteLink toàn cầu cho môi trường Production và Development.*

---

## Lợi ích

Việc triển khai **AWS Direct Connect SiteLink** mang lại các lợi ích chính sau:

- **Đơn giản hóa quản lý mạng:** loại bỏ sự phức tạp của định tuyến MPLS Layer 3 VPN  
- **Tăng độ ổn định:** tận dụng mạng backbone AWS để cải thiện khả năng phục hồi và giảm độ trễ trung bình 15%  
- **Cải thiện trải nghiệm người dùng:** nhờ độ trễ thấp hơn và nhất quán hơn giữa các trung tâm dữ liệu  
- **Giám sát toàn diện:** thông qua **Amazon CloudWatch Network Synthetic Monitor** và các công cụ giám sát tổng thể  
- **Bảo mật nâng cao:** sử dụng **MACSec encryption (Layer 2)** cho toàn bộ kết nối Direct Connect  

Triển khai SiteLink được thực hiện theo từng giai đoạn:
1. **Giai đoạn 1:** SiteLink được dùng như **giải pháp dự phòng** cho mạng riêng toàn cầu hiện có  
2. **Giai đoạn 2:** Chuyển SiteLink thành **kết nối chính**, loại bỏ các kết nối điểm-điểm cũ  

Kết quả: Salesforce đạt được một **mạng lưới toàn cầu đáng tin cậy, bảo mật, và dễ mở rộng hơn**.

---

## Trích dẫn từ Salesforce

> “Với SiteLink, Salesforce Business Technology đã có thể hợp lý hóa các hoạt động mạng và đảm bảo khả năng phục hồi tối đa cho kết nối đường trục toàn cầu của chúng tôi.  
> SiteLink dễ dàng kích hoạt trên các mạch Direct Connect hiện có. Điều này cho phép chúng tôi thiết lập kết nối giữa bảy trung tâm dữ liệu toàn cầu chỉ trong vài phút và đáp ứng nhu cầu mạng cho các cơ hội thị trường trong tương lai một cách nhanh chóng.”  
> — *Ravi Patel, Giám đốc Kỹ thuật Cấp cao tại Salesforce.*

---

## Kết luận

Qua bài đăng này, chúng ta thấy cách **Salesforce Business Technology** sử dụng **AWS Direct Connect SiteLink** để:
- Hợp nhất kiến trúc mạng trên phạm vi toàn cầu  
- Hiện đại hóa kết nối để giảm chi phí và độ phức tạp vận hành  
- Nâng cao hiệu suất, bảo mật, và khả năng phục hồi  

**SiteLink** giúp Salesforce xây dựng nền tảng kết nối linh hoạt, sẵn sàng cho **mở rộng toàn cầu**, đồng thời duy trì **hiệu quả kinh tế và hiệu suất tối ưu**.

---

## Giới thiệu về các tác giả

**Alexandra Huides** — Kiến trúc sư giải pháp chuyên gia mạng chính tại AWS.  
Cô tập trung vào việc giúp khách hàng xây dựng kiến trúc mạng mở rộng linh hoạt và là diễn giả về IPv6.

**Corey Harris Jr.** — Kiến trúc sư giải pháp cấp cao tại AWS, tập trung hỗ trợ Salesforce triển khai và tối ưu hóa các giải pháp AWS.

**Georgi Stoev** — Kiến trúc sư kỹ thuật cấp cao tại Salesforce, chuyên về Multi-cloud, AI, Security và Network Infrastructure.

**Ravi Patel** — Giám đốc kỹ thuật cấp cao tại Salesforce, với hơn 15 năm kinh nghiệm trong việc xây dựng các mạng hiệu suất cao, linh hoạt và bảo mật.
