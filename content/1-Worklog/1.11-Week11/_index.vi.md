---
title: "Worklog Tuần 11"
date: 2026-06-29
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu Tuần 11:
- **Mục tiêu hàng tuần:** Tách biệt logic chấm điểm khỏi yêu cầu nộp bài bằng cách sử dụng SQS Grading Queue (Hàng đợi chấm điểm) và Lambda Grading Worker.  
- **Kết quả đạt được:** Backend lưu bài nộp với trạng thái đang chấm điểm (grading status), gửi một tác vụ (job) đến SQS, và worker xử lý việc chấm điểm/cập nhật kết quả vào MongoDB.

### Các nhiệm vụ thực hiện trong tuần này:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | - **Khởi tạo Hàng đợi:** <br>&emsp; + Tạo SQS Grading Queue <br>&emsp; + Cấu hình Dead-Letter Queue (DLQ - Hàng đợi thư chết) cho các tác vụ chấm điểm thất bại | 29/06/2026 | 29/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - **Tái cấu trúc Backend:** <br>&emsp; + Cập nhật Express API để lưu các bài nộp ban đầu với trạng thái 'đang chấm điểm' (grading) <br>&emsp; + Tích hợp AWS SDK để đẩy các tác vụ lên SQS | 29/06/2026 | 29/06/2026 | Internal Project Docs |
| 3 | - **Thiết lập Lambda:** <br>&emsp; + Khởi tạo Lambda Grading Worker <br>&emsp; + Cấu hình các IAM role để cấp quyền đọc SQS và quyền ghi vào MongoDB | 30/06/2026 | 30/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - **Triển khai Logic chấm điểm:** <br>&emsp; + Viết logic cho Lambda để xử lý các message từ SQS và tính điểm <br>&emsp; + Kết nối Lambda với MongoDB để cập nhật kết quả | 01/07/2026 | 01/07/2026 | Internal Project Docs |
| 5 | - **Kiểm thử Toàn trình (End-to-End):** <br>&emsp; + Kiểm thử luồng nộp bài bất đồng bộ từ frontend đến cơ sở dữ liệu <br>&emsp; + Xác minh việc xử lý và xóa message trên SQS | 02/07/2026 | 02/07/2026 | Internal Project Docs |

### Thành quả Tuần 11:
* Tách biệt thành công logic chấm điểm nặng nề khỏi luồng nộp bài tức thời của người dùng bằng cách sử dụng Amazon SQS.
* Cải thiện thời gian phản hồi của API nhờ việc backend trả về ngay kết quả thành công trong khi lưu trạng thái tạm thời "đang chấm điểm" (grading) vào cơ sở dữ liệu.
* Khởi tạo và cấu hình bảo mật thành công SQS Grading Queue để đệm (buffer) các tác vụ nộp bài, đảm bảo không mất dữ liệu khi lưu lượng truy cập tăng đột biến.
* Phát triển và triển khai một Lambda Grading Worker chuyên dụng có khả năng tự động mở rộng để xử lý các message từ hàng đợi.
* Xác minh rằng Lambda worker tính điểm chính xác và cập nhật thành công kết quả chấm điểm cuối cùng trực tiếp vào MongoDB.