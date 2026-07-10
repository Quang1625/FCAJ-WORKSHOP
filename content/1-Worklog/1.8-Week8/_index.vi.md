---
title: "Nhật ký công việc Tuần 8"
date: 2026-06-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu Tuần 8:
* Hoàn thiện tương tác Frontend cho hệ thống Serverless.
* Tìm hiểu trách nhiệm bảo mật và các công cụ giám sát trên AWS (Bảo mật cốt lõi - Tuần 1).
* Xác định phạm vi MVP (Sản phẩm khả dụng tối thiểu), đánh giá mã nguồn hiện tại và chốt kiến trúc AWS Serverless Hybrid cho dự án Examora.
* Triển khai xác thực với Cognito/SES, triển khai (deploy) Express backend lên Lambda và bảo mật các API bằng API Gateway JWT Authorizer.

### Nhóm Workshop
* Mục tiêu của tuần là xác định phạm vi MVP, đánh giá mã nguồn hiện tại và chốt kiến trúc AWS Serverless Hybrid cho Examora.
* Kết quả đạt được là nắm bắt được cấu trúc frontend/backend, quyết định giữ lại các module nào, chuyển các module nào lên AWS, và có một backlog (danh sách công việc) triển khai ban đầu.

### Các nhiệm vụ thực hiện trong tuần này:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | - **Bảo mật cốt lõi:** Tìm hiểu về Mô hình Trách nhiệm Chia sẻ của AWS và các công cụ giám sát (Amazon CloudWatch & AWS CloudTrail) | 01/06/2026 | 01/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - **Nhóm Workshop - Đánh giá mã nguồn:** Đi sâu tìm hiểu mã nguồn frontend và backend hiện tại của Examora để nắm bắt cấu trúc và luồng dữ liệu sẵn có | 02/06/2026 | 02/06/2026 | <https://docs.aws.amazon.com/apigateway/> |
| 3 | - **Nhóm Workshop - Kiến trúc:** Xác định phạm vi MVP, quyết định module nào sẽ giữ lại ở hệ thống hiện tại, và module nào sẽ chuyển sang mô hình AWS Serverless Hybrid | 03/06/2026 | 03/06/2026 | ExamoraServerless/01_Examora_KienTruc_Serverless.md |
| 4 | - **Chuyển đổi Backend & Xác thực:** Tạo backlog triển khai ban đầu. Cấu hình Amazon Cognito/SES và triển khai backend Express đã được tái cấu trúc lên AWS Lambda | 04/06/2026 | 04/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - **Bảo mật Frontend & API:** Kết nối frontend với các API serverless và bảo mật các endpoint sử dụng Amazon API Gateway JWT Authorizer | 05/06/2026 | 05/06/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Thành quả Tuần 8:
* Nắm vững kiến thức về trách nhiệm bảo mật trên AWS và các dịch vụ giám sát cốt lõi.
* Rà soát thành công mã nguồn frontend và backend hiện tại của Examora để thiết lập bản đồ các phụ thuộc (dependencies).
* Chốt được phạm vi MVP và đưa ra các quyết định chiến lược về kiến trúc đối với các module sẽ được đưa lên AWS.
* Lập thảo thành công một backlog triển khai chi tiết và có tính thực thi cao cho kiến trúc Serverless Hybrid mới.
* Tích hợp Amazon Cognito và SES để quản lý và bảo mật luồng xác thực cũng như thông báo tới người dùng.
* Triển khai thành công ứng dụng Express lên AWS Lambda và bảo mật toàn bộ tương tác API bằng JWT Authorizer.