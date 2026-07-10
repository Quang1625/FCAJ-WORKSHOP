---
title: "Worklog Tuần 10"
date: 2026-06-23
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu Tuần 10:
- Chuyển đổi luồng tải lên tệp tin sang S3 Upload Bucket sử dụng presigned URLs (URL được ký trước).
- Tách tính năng import (nhập) tài liệu Word thành một hàm AWS Lambda để xử lý bất đồng bộ.

### Các nhiệm vụ thực hiện trong tuần này:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | - **Cấu hình Backend & S3:** <br>&emsp; + Cấu hình CORS và các chính sách IAM cho S3 bucket <br>&emsp; + Triển khai API backend để tạo các S3 presigned URLs | 23/06/2026 | 23/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - **Tích hợp Frontend:** <br>&emsp; + Cập nhật ứng dụng frontend để gọi API lấy presigned URLs và tải tệp trực tiếp lên S3 <br>&emsp; + Xác minh các S3 prefix (cấu trúc thư mục) | 24/06/2026 | 24/06/2026 |  <https://docs.aws.amazon.com/AmazonS3/latest/userguide/notification-how-to-event-types-and-destinations.html>|
| 3 | - **Khởi tạo Lambda:** <br>&emsp; + Tạo hàm Word Import Lambda <br>&emsp; + Thiết lập gói triển khai (deployment package) với các thư viện phân tích (parsing) tệp `.docx` | 25/06/2026 | 25/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - **Logic phân tích & Cơ sở dữ liệu:** <br>&emsp; + Viết logic trên Lambda để phân tích nội dung `.docx` <br>&emsp; + Kết nối Lambda với MongoDB và ánh xạ (map) các schema dữ liệu câu hỏi | 26/06/2026 | 26/06/2026 | <https://docs.aws.amazon.com/lambda/>  |
| 5 | - **Kiểm thử Toàn trình (End-to-End):** <br>&emsp; + Kiểm thử toàn bộ luồng tải lên và đường ống (pipeline) import bất đồng bộ <br>&emsp; + Xác thực tính toàn vẹn của dữ liệu trong MongoDB | 27/06/2026 | 27/06/2026 | Internal Project Docs |

### Thành quả Tuần 10:
* Chuyển đổi thành công luồng tải lên tệp tin chính sang sử dụng S3 presigned URLs, giúp giảm tải lưu lượng truyền tệp nặng cho backend cốt lõi.
* Xác minh rằng tất cả các tệp được tải lên đều được phân loại hợp lý và lưu vào đúng các S3 prefix (cấu trúc thư mục).
* Tách biệt thành công tác vụ xử lý tài liệu Word nặng nề bằng cách chuyển nó sang một hàm AWS Lambda chuyên dụng và chạy bất đồng bộ.
* Hàm Word Import Lambda hoạt động trơn tru: phân tích chính xác các tệp `.docx`, cấu trúc lại dữ liệu và lưu thành công các câu hỏi được trích xuất vào cơ sở dữ liệu MongoDB.