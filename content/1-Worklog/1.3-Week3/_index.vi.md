---
title: "Worklog Tuần 3"
date: 2026-04-27
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu Tuần 3:

- **Kết nối cộng đồng:** Giao lưu và thiết lập mối quan hệ với các thành viên trong chương trình First Cloud AI Journey.
- **Làm chủ kiến thức cơ bản về AWS:** Hiểu rõ về các dịch vụ AWS cốt lõi và sử dụng thành thạo giao diện điều khiển (Management Console) cũng như giao diện dòng lệnh (CLI).
- **Nâng cao bảo mật đám mây:** Củng cố kiến thức bảo mật tài khoản và triển khai các chiến lược quản lý danh tính & truy cập nâng cao bằng AWS IAM.
- **Đi sâu vào mạng ảo:** Nghiên cứu lý thuyết và thực hành triển khai các kiến trúc Amazon Virtual Private Cloud (VPC).
- **Thực hành bảo vệ cơ sở hạ tầng:** Tạo các subnet (phân mạng), thiết lập route table (bảng định tuyến) và cấu hình Security Groups (nhóm bảo mật) để bảo vệ tài nguyên đám mây một cách hiệu quả.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Nghiên cứu sâu về quản lý danh tính và bảo mật người dùng trên hệ thống <br> - Tìm hiểu cách thiết lập Xác thực đa yếu tố (MFA) cho tài khoản | 4/5/2026 | 4/5/2026 | Khóa học First Cloud AI Journey |
| 3 | - Thực hành phân quyền trong IAM, quản lý nhóm người dùng và cô lập đặc quyền giữa Root User và IAM Users <br> - Tạo các tài khoản phụ phục vụ cho các tác vụ vận hành hàng ngày | 5/5/2026 | 5/5/2026 | Khóa học First Cloud AI Journey |
| 4 | - Học lý thuyết cốt lõi của Module 02 về Amazon Virtual Private Cloud (VPC) <br> - Khám phá các khái niệm cơ bản: VPC là gì, public subnet và private subnet | 6/5/2026 | 6/5/2026 | Khóa học First Cloud AI Journey |
| 5 | - Tìm hiểu về cơ chế định tuyến mạng thông qua Route Tables và Internet Gateways <br> - Nghiên cứu giải pháp NAT Gateway cho phép các tài nguyên trong private subnet kết nối một chiều ra internet | 7/5/2026 | 7/5/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Thiết kế sơ đồ kiến trúc mạng cho bài thực hành Lab <br> - Chuẩn bị dải IPv4 CIDR cho VPC và các subnet dự kiến khởi tạo | 8/5/2026 | 8/5/2026 | Khóa học First Cloud AI Journey |
| 7 | - Thực hiện bài Lab thực hành trên AWS Management Console <br> - Khởi tạo VPC, phân chia public/private subnets, gắn Internet Gateway, cấu hình Route Tables và thiết lập các quy tắc tường lửa với Security Groups | 9/5/2026 | 9/5/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 3:

| Thứ | Công việc | Kết quả đạt được | Hình ảnh |
| --- | --- | --- | --- |
| 2 | Cấu hình Xác thực đa yếu tố (MFA) | Cấu hình thành công Xác thực đa yếu tố (MFA) cho môi trường tài khoản, tăng cường lá chắn bảo mật cho hệ thống. | ![MFA](image.png) |
| 3 | Quản lý tài khoản & phân quyền IAM | Đảm bảo an toàn cho Root User bằng cách vô hiệu hóa các access key đang hoạt động. Quản lý và phân phối quyền hạn cho tài khoản phụ truc-user trong nhóm Admin-groups phục vụ vận hành hàng ngày đúng quy định. | ![IAM](image-3.png) |
| 4 | Lý thuyết nền tảng Amazon VPC | Hiểu rõ bản chất cô lập logic của Virtual Private Cloud (VPC) để phân tách các môi trường phát triển (dev, test, production). Làm chủ việc phân chia không gian mạng thành public subnet và private subnet. | _(Sơ đồ kiến trúc mạng Amazon VPC)_ |
| 5 | Nghiên cứu cơ chế định tuyến mạng | Thấu hiểu cơ chế hoạt động của Default route table và Custom route table. Biết cách sử dụng Internet Gateway để mở cổng kết nối internet hướng ra ngoài và cách NAT Gateway giúp kết nối an toàn cho tài nguyên private subnet một chiều. | _(Hình minh họa cấu hình định tuyến hệ thống)_ |
| 6 | Lập kế hoạch phân bổ tài nguyên hạ tầng | Xác định rõ ràng các tham số kỹ thuật, dải CIDR 10.0.0.0/16 và lập kế hoạch liên kết rõ ràng cho các thành phần mạng trước khi triển khai thực tế trên console. | _(Hình minh họa bảng phân bổ IP bài Lab)_ |
| 7 | Triển khai thực tế Lab 03 (VPC deployment) | Khởi tạo thành công mạng ảo tên là truc-vpc (IPv4 CIDR 10.0.0.0/16). Hoàn tất cấu hình chi tiết cho truc-public-subnet1 và truc-private-subnet1. Gắn cổng truc-igw, tạo bảng định tuyến truc-route-Public1 và thiết lập hai security groups cho phép quản lý an toàn các giao thức SSH, Ping và HTTP. | ![Your VPCs](image-1.png) ![Subnets](image-2.png) |
