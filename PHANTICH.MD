# Phân tích cấu hình Logback cho Dev và Production

## Môi trường Dev
- Mục tiêu chính là hỗ trợ Developer debug nhanh.
- Log nên in trực tiếp ra Console để dễ quan sát khi chạy ứng dụng.
- Sử dụng mức DEBUG để hiển thị nhiều thông tin chi tiết phục vụ phát triển.

## Môi trường Production
- Mục tiêu chính là ổn định, lưu vết và tiết kiệm tài nguyên server.
- Log cần lưu ra file để phục vụ kiểm tra lỗi và audit hệ thống.
- Sử dụng mức INFO để giảm lượng log không cần thiết.
- Cần cơ chế Rolling File để tự động cắt và nén log tránh đầy ổ cứng.
- Giữ log tối đa 30 ngày để phục vụ truy vết sự cố.