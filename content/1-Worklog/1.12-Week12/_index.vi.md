---
title: "Worklog Tuần 12"
date: 2026-06-29
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu Tuần 12:
* **Mục tiêu hàng tuần:** Triển khai frontend trên Amplify Hosting, thiết lập Route 53/tên miền, và hoàn thành kiểm thử, tài liệu đề xuất (proposal) cùng với báo cáo workshop.
* **Kết quả đạt được:** Frontend đang chạy trên Amplify, CORS đã hỗ trợ local/Amplify/tên miền, các luồng làm việc chính đã được kiểm thử lại, và tài liệu đã được cập nhật theo kiến trúc mới.

### Các nhiệm vụ thực hiện trong tuần này:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | - **Triển khai Frontend:** <br>&emsp; + Kết nối repository với AWS Amplify Hosting <br>&emsp; + Cấu hình thiết lập build và triển khai ứng dụng frontend | 29/06/2026 | 29/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - **Quản lý Tên miền & DNS:** <br>&emsp; + Đăng ký/cấu hình tên miền tùy chỉnh sử dụng Amazon Route 53 <br>&emsp; + Gắn tên miền tùy chỉnh vào bản triển khai trên Amplify | 30/06/2026 | 30/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - **Cấu hình CORS & Bảo mật:** <br>&emsp; + Cập nhật chính sách CORS của backend API để chấp nhận request từ localhost, URL mặc định của Amplify và tên miền tùy chỉnh | 01/07/2026 | 01/07/2026 | Internal Project Docs |
| 4 | - **Kiểm thử lại Hệ thống:** <br>&emsp; + Tiến hành kiểm thử toàn trình (end-to-end) tất cả các luồng ứng dụng chính trên môi trường thực tế (production) <br>&emsp; + Khắc phục mọi lỗi (bug) liên quan đến UI/API | 02/07/2026 | 02/07/2026 | Internal Project Docs |
| 5 | - **Tài liệu hóa & Báo cáo:** <br>&emsp; + Cập nhật sơ đồ kiến trúc hệ thống để phản ánh cấu hình cuối cùng <br>&emsp; + Hoàn thành đề xuất dự án và báo cáo workshop | 03/07/2026 | 03/07/2026 | Internal Project Docs |

### Thành quả Tuần 12:
* Triển khai thành công ứng dụng frontend lên AWS Amplify Hosting, thiết lập một đường ống triển khai liên tục (continuous deployment pipeline) đáng tin cậy.
* Cấu hình Amazon Route 53 để quản lý DNS và gắn thành công một tên miền tùy chỉnh cho frontend trên môi trường production.
* Giải quyết các hạn chế về chia sẻ tài nguyên chéo nguồn bằng cách cập nhật đúng cấu hình CORS của backend để hỗ trợ môi trường phát triển cục bộ (local), URL của Amplify và tên miền thực tế.
* Thực hiện kiểm thử lại toàn diện các luồng công việc chính (xác thực, nộp bài, chấm điểm bất đồng bộ, tải lên tệp tin) trên môi trường live (thực tế), xác nhận tính ổn định của hệ thống.
* Hoàn thiện và trau chuốt toàn bộ tài liệu dự án, bao gồm đề xuất kỹ thuật và báo cáo workshop chi tiết, thể hiện đầy đủ kiến trúc AWS Serverless Hybrid mới.