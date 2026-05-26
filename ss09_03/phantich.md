# Phân tích Lombok & Parameterized Logging

Sử dụng Parameterized Logging với {} tối ưu hiệu năng hơn dấu + vì:

- Dấu + sẽ nối chuỗi ngay lập tức, kể cả khi log level không được ghi, gây tốn CPU và bộ nhớ không cần thiết.

- Parameterized Logging ({}) chỉ thực hiện thay thế giá trị khi log level được bật, giúp tối ưu hiệu năng hệ thống.

- Code ngắn gọn, dễ đọc và tránh lỗi copy-paste khi log nhiều biến.