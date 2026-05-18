# 🎓 Nền tảng Thi thử & Luyện thi TOEIC/IELTS Trực tuyến

🇺🇸 English version: [README.md](./README.md)

---

Đây là một hệ thống **EdTech toàn diện**, mô phỏng các bài thi chuẩn hóa quốc tế như **TOEIC** và **IELTS**.

Hệ thống tập trung vào:

- Giao diện tối giản, hiện đại
- Trải nghiệm người dùng mượt mà
- Hiệu năng và khả năng chịu tải cao
- Hoạt động ổn định 24/7

Dự án áp dụng kiến trúc **Micro-repositories** nhằm tách biệt các miền nghiệp vụ, giúp dễ dàng bảo trì và mở rộng trong tương lai.

---

# 🏗 Cấu trúc Hệ thống (Repositories)

Đây là repository trung tâm mô tả kiến trúc tổng thể của hệ sinh thái.

Hệ thống được chia thành 3 repositories độc lập:

| Module | Mô tả | Repository |
|---|---|---|
| API Server | Backend cung cấp RESTful API, xử lý chấm điểm, quản lý phiên thi và đồng bộ dữ liệu | [API_Repo_Link](github.com/dangLuan01/ets-api) |
| Client App | Frontend dành cho học viên, xử lý giao diện làm bài, luyện tập và thống kê | [Client_Repo_Link](https://github.com/dangLuan01/ets-client) |
| Admin Portal | Trang quản trị nội dung (CMS), quản lý đề thi, câu hỏi và người dùng | [Admin_Repo_Link](https://github.com/dangLuan01/ets-admin) |

---

# 🚀 Tính năng Cốt lõi

## Flexible Exam Engine

Hỗ trợ nhiều chế độ học tập trên cùng một giao diện linh hoạt.

### Exam Mode

Mô phỏng áp lực phòng thi thực tế:

- Đề thi 100–200 câu
- Luồng tính điểm chuẩn hóa
- Giao diện tối ưu cho thi thật

### Practice Mode

Áp dụng triết lý Micro-learning:

- Hiển thị đáp án tức thì
- Có giải thích chi tiết
- Hỗ trợ luyện theo từng part

### Review Mode

Hệ thống xem lại bài thi chi tiết:

- Xem lịch sử làm bài
- Phân tích điểm mạnh/yếu
- Theo dõi tiến độ học tập

---

## Seamless Cross-Device Experience

Đồng bộ trạng thái theo thời gian thực:

- Bắt đầu trên điện thoại
- Tiếp tục trên máy tính
- Không gián đoạn phiên làm bài

---

## Resilient Auto-Save

Cơ chế tự động lưu tiến trình thông minh:

- Kiến trúc Zero-Data Loss
- Không mất dữ liệu khi:
  - Mất mạng
  - Treo trình duyệt
  - Tắt máy đột ngột

---

## Smart Revision

Hệ thống bookmark & ôn tập thông minh:

- Lưu câu hỏi quan trọng
- Cá nhân hóa quá trình ôn tập
- Nền tảng cho Spaced Repetition

---

# 🛠 Điểm nhấn Kiến trúc

## Data-Driven UI

Frontend được thiết kế theo hướng dữ liệu điều khiển giao diện.

Components có thể tự thích nghi với:

- Đề Full
- Mini Test
- Luyện Part

Ưu điểm:

- Tái sử dụng cao
- Hạn chế hard-code
- Dễ mở rộng tính năng

---

## Optimized Database Writes

Backend tối ưu cho lượng lớn thao tác chọn đáp án đồng thời.

Kỹ thuật áp dụng:

- Batching & Queueing
- Bulk Upsert
- Giảm áp lực Database
- Tăng throughput hệ thống

---

## Stateless & Scalable Backend

Backend được thiết kế phi trạng thái:

- Dễ scale ngang
- Sẵn sàng multi-instance
- Chịu tải cao

---

# 💻 Công nghệ Sử dụng

## Backend

- Go (Golang)
- Gin Framework

## Frontend

- React
- Next.js
- Zustand

## Database & Caching

- MySQL / PostgreSQL
- Redis

## DevOps & Deployment

- Docker
- Nginx
- GitHub Actions (CI/CD)
- Linux VPS
