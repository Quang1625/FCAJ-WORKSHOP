---
title: "Worklog Tuần 9"
date: 2026-06-16
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu Tuần 9:
- Chuyển đổi luồng tải lên tệp tin sang S3 Upload Bucket sử dụng presigned URLs (URL được ký trước) và tách tính năng import (nhập) tệp Word thành một hàm Lambda bất đồng bộ.
- Tách biệt logic chấm điểm khỏi yêu cầu nộp bài thi bằng cách sử dụng SQS Grading Queue (Hàng đợi chấm điểm) và Lambda Grading Worker.  
- Tách biệt logic tạo tệp PDF khỏi yêu cầu nộp bài thi bằng cách sử dụng SQS PDF Generation Queue (Hàng đợi tạo PDF) và Lambda PDF Generation Worker.  
- Tách biệt logic thông báo qua email khỏi yêu cầu nộp bài thi bằng cách sử dụng SQS Email Notification Queue (Hàng đợi thông báo Email) và Lambda Email Notification Worker.

### Nhóm Workshop
- **Mục tiêu hàng tuần:** Triển khai xác thực với Cognito/SES, triển khai (deploy) Express backend lên Lambda và bảo vệ các API bằng API Gateway JWT Authorizer.
- **Kết quả đạt được:** Hoàn thành luồng đăng ký, mã OTP qua email, đăng nhập, đồng bộ hồ sơ người dùng với MongoDB, Lambda Backend API và kiểm thử API Gateway cơ bản.

### Các nhiệm vụ thực hiện trong tuần này:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | - **Nhóm Workshop - Luồng xác thực:** Triển khai đăng ký người dùng, xác thực OTP qua email sử dụng Amazon SES, và luồng đăng nhập sử dụng Amazon Cognito <br>&emsp; + Đồng bộ hồ sơ người dùng với MongoDB | 16/06/2026 | 16/06/2026 | <https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api.html/> |
| 2 | - **Nhóm Workshop - Backend & API:** Triển khai Express backend lên AWS Lambda <br>&emsp; + Cấu hình API Gateway JWT Authorizer và tiến hành kiểm thử các endpoint cơ bản | 17/06/2026 | 17/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - **Tải lên & Import tệp tin:** Chuyển đổi luồng tải lên tệp sang S3 sử dụng presigned URLs <br>&emsp; + Tách và tái cấu trúc (refactor) tính năng import tệp Word thành một hàm Lambda bất đồng bộ | 18/06/2026 | 18/06/2026 | <https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-jwt-authorizer.html/> |
| 4 | - **Tách biệt Chấm điểm & PDF:** Khởi tạo các hàng đợi SQS cho luồng Chấm điểm và Tạo PDF <br>&emsp; + Phát triển và gắn các Lambda Worker để xử lý các tác vụ từ các hàng đợi tương ứng | 19/06/2026 | 19/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - **Tách biệt Email:** Khởi tạo SQS Email Notification Queue (Hàng đợi thông báo Email) <br>&emsp; + Phát triển Lambda Email Notification Worker và kiểm thử toàn trình luồng nộp bài đã được tách biệt hoàn toàn | 20/06/2026 | 20/06/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Thành quả Tuần 9:
* Hoàn thành xuất sắc quy trình xác thực người dùng, bao gồm đăng ký, xác minh OTP qua email bằng SES và đăng nhập qua Cognito.
* Thiết lập việc đồng bộ dữ liệu liền mạch giữa tầng xác thực và hồ sơ người dùng được lưu trữ trong cơ sở dữ liệu MongoDB.
* Triển khai Express backend dưới dạng serverless API trên AWS Lambda và bảo vệ thành công các endpoint bằng API Gateway JWT Authorizer.
* Tối ưu hóa hiệu suất ứng dụng bằng cách chuyển luồng tải lên tệp tin trực tiếp sang S3 thông qua presigned URLs và di chuyển tác vụ nặng (nhập tệp Word) sang một hàm Lambda chạy ngầm.
* Thiết kế một kiến trúc nộp bài thi tách biệt cao độ, sử dụng Amazon SQS để xử lý các tác vụ chấm điểm, tạo PDF và thông báo qua email một cách bất đồng bộ.
* Phát triển và triển khai các Lambda Worker chuyên dụng cho từng hàng đợi SQS, đảm bảo API cốt lõi luôn phản hồi nhanh và không bị nghẽn (non-blocking) đối với người dùng cuối.