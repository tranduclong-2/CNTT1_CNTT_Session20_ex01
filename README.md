# Bài 1 : Xử lý cảnh báo đăng nhập giả mạo GitHub

1. Chỉ ra ký tự lạ trong URL
URL được cung cấp: https://githúb.com/login
- Ký tự lạ là ú trong từ githúb.
- Đây là ký tự Unicode, có dấu, khác với chữ u thông thường trong tên miền github.com.
- Kẻ xấu sử dụng ký tự trông gần giống chữ bình thường để tạo địa chỉ giả mạo.
- Người dùng có thể không nhận ra sự khác biệt và tưởng rằng mình đang truy cập GitHub thật.
Đây là hình thức tấn công Homograph Attack (tấn công giả mạo ký tự).

Cảnh báo
 Không nhập mật khẩu vào địa chỉ githúb.com.
2. Quy trình kiểm tra URL
| Bước | Cách thực hiện |
| --- | --- |
| 1 | Kiểm tra tên miền	Quan sát kỹ từng ký tự, đặc biệt là chữ có dấu hoặc ký tự lạ |
| 2 | So sánh địa chỉ	Địa chỉ GitHub chính thức là github.com |
| 3 | Dùng công cụ hỗ trợ	Sử dụng VirusTotal để kiểm tra URL đáng ngờ |
| 4 | Truy cập an toàn tự nhập https://github.com vào trình duyệt thay vì nhấn vào liên kết trong email |
