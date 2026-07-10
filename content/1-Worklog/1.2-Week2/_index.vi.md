---
title: "Worklog Tuần 2"
date: 2026-04-20
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---


### Mục tiêu tuần 2


* **Hoàn tất các bài tập trên AWS Console**: Thu thập tổng cộng **$200 USD AWS Credits** để tối ưu chi phí trong quá trình thực hành với các dịch vụ có tính phí.
* **Tổng quan hóa hệ sinh thái dịch vụ AWS**: Tìm hiểu các nhóm dịch vụ chính (*Compute, Storage, Networking, Database*, v.v.), kiến trúc hệ thống và cách tính phí của AWS nhằm chuẩn bị cho việc thiết kế, triển khai hạ tầng tối ưu và tiết kiệm trong tương lai.

---

###  Các công việc cần triển khai trong tuần này

| Thứ | Hạng mục công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu tham khảo |
| :---: | :--- | :---: | :---: | :--- |
| **3** | - Tìm hiểu giao diện AWS Management Console <br> - Cài đặt và cấu hình AWS CLI trên máy tính cá nhân (*Access Key, Secret Key, Default Region*) <br> - Thực hành: Sử dụng các lệnh AWS CLI cơ bản | 21/04/2026 | 21/04/2026 | [AWS Cloud Journey](https://cloudjourney.awsstudygroup.com/) |
| **4** | - Tìm hiểu dịch vụ Amazon EC2 cơ bản: *Instance types, AMI, EBS, Elastic IP* <br> - Nghiên cứu các phương thức kết nối SSH từ máy trạm vào EC2 | 22/04/2026 | 22/04/2026 | [AWS Cloud Journey](https://cloudjourney.awsstudygroup.com/) |
| **5** | - **Thực hành Lab kỹ thuật**: <br>&emsp; + Khởi tạo EC2 instance hoàn chỉnh <br>&emsp; + Tạo và gắn thêm EBS volume <br>&emsp; + Thực hiện kết nối SSH và quản lý tài nguyên song song qua Console & CLI | 23/04/2026 | 23/04/2026 | [AWS Cloud Journey](https://cloudjourney.awsstudygroup.com/) |

---

###  Kết quả đạt được tuần 2

| Thứ | Hạng mục | Kết quả đạt được chi tiết | Minh chứng / Hình ảnh |
| :---: | :--- | :--- | :---: |
| **3** | **Tương tác & Cấu hình CLI** | Học **Module 1 (Phần 2: Cách Thức Tương Tác Với AWS)**: <br> Hiểu rõ 3 cách điều khiển dịch vụ của AWS: <br> - **AWS Management Console**: Giao diện Web. Phân biệt tài khoản *Root User* (bảo mật với MFA, không dùng hằng ngày) và *IAM User* (tài khoản phụ dùng hằng ngày với ID riêng). <br> - **AWS CLI**: Giao diện dòng lệnh giúp thao tác nhanh. Đã cài đặt hoàn chỉnh trên máy, cấu hình *Access Key* và *Secret Key* an toàn (không push lên GitHub). <br> - **AWS SDK**: Bộ công cụ lập trình (Python, Java...) gọi API trực tiếp từ code. | *(Hình ảnh terminal CLI hoặc file config)* |
| **4** | **Kiến trúc máy chủ EC2** | Nắm vững lý thuyết về *Instance types*, các loại *AMI*, ổ lưu trữ *EBS* và các cơ chế định tuyến IP, bảo mật hệ thống thông qua *SSH Key Pair*. | *(Hình ảnh giao diện EC2 Console)* |
| **5** | **Thực hành Lab triển khai** | Khởi tạo thành công máy chủ EC2, tạo và gắn thêm EBS volume, kết nối SSH từ máy cá nhân ổn định; kết hợp quản lý tài nguyên song song qua cả Console & CLI. | *(Hình ảnh SSH thành công vào EC2)* |
