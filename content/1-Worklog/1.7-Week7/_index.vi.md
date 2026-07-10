---
title: "Nhật ký công việc Tuần 7"
date: 2026-05-25
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu Tuần 7:
* Làm quen với kiến trúc Serverless (Không máy chủ), AWS Lambda và API Gateway.
* Triển khai một Backend serverless cơ bản.
* Nắm bắt các khái niệm về cơ sở dữ liệu NoSQL (DynamoDB).
* Quản lý danh tính người dùng và xác thực ứng dụng.

### Các nhiệm vụ thực hiện trong tuần này:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | - Tìm hiểu nền tảng kiến trúc Serverless <br> - Hiểu các mô hình thực thi của AWS Lambda <br> - **Thực hành:** Tạo và kiểm thử một hàm Lambda "Hello World" đơn giản | 25/05/2026 | 25/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Tìm hiểu các khái niệm về Amazon API Gateway (REST APIs, HTTP APIs, Endpoints) <br> - **Thực hành:** Kết nối API Gateway với AWS Lambda để kích hoạt hàm thông qua HTTP request | 26/05/2026 | 26/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Tìm hiểu cơ bản về NoSQL và Amazon DynamoDB: <br>&emsp; + Partition keys (Khóa phân vùng) và Sort keys (Khóa sắp xếp) <br>&emsp; + Các chế độ công suất đọc/ghi (Read/Write capacity modes) <br> - **Thực hành:** Tạo một bảng DynamoDB | 27/05/2026 | 27/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - **Thực hành:** Cập nhật hàm Lambda để đọc và ghi dữ liệu vào bảng DynamoDB, hoàn thiện backend serverless | 28/05/2026 | 28/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Tìm hiểu Amazon Cognito để quản lý danh tính <br> - **Thực hành:** <br>&emsp; + Tạo một Cognito User Pool <br>&emsp; + Bảo mật API Gateway sử dụng Cognito Authorizer | 29/05/2026 | 29/05/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Thành quả Tuần 7:
* Hiểu các nguyên tắc cốt lõi của điện toán không máy chủ (serverless computing) và kiến trúc hướng sự kiện (event-driven) trên AWS.
* Viết và triển khai thành công một hàm AWS Lambda để thực thi mã backend mà không cần cấp phép hay quản lý máy chủ.
* Cấu hình Amazon API Gateway để định tuyến các HTTP request tới hàm Lambda, thiết lập một RESTful serverless API hoạt động đầy đủ.
* Nắm vững các nền tảng cơ bản của cơ sở dữ liệu NoSQL và khởi tạo một bảng Amazon DynamoDB để lưu trữ dữ liệu nhanh chóng, linh hoạt và có khả năng mở rộng.
* Tạo một Amazon Cognito User Pool để xử lý việc đăng ký và đăng nhập của người dùng.
* Tích hợp thành công Amazon Cognito với API Gateway để hạn chế quyền truy cập API chỉ dành cho những người dùng đã được xác thực.