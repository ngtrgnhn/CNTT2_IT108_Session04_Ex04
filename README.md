<p align="center">
  <a href="https://ptit.edu.vn" target="_blank">
    <img src="./images/ptit.svg" alt="PTIT Logo" height="60" style="border-radius: 8px; padding: 4px; background: #ffffff;" />
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <span style="font-size: 30px; font-weight: bold; color: #888;">✕</span>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://rikkei.edu.vn" target="_blank">
    <img src="./images/rikkei-logo.webp" alt="Rikkei Edu Logo" height="60" style="border-radius: 8px; padding: 4px; background: #ffffff;" />
  </a>
</p>

## Phần 1: Phân tích & Đề xuất

| Tiêu chí | Cách 1: Đường dẫn tuyệt đối (C:\\Users\\An\\...) | Cách 2: Đường dẫn tương đối (../Data/users.csv) |
| :---- | :---- | :---- |
| Tính di động (Portability) | Kém: Bị gắn cứng (hard-code) theo ổ đĩa và tên tài khoản người dùng (C:\\, An). Sẽ báo lỗi ngay lập tức khi chuyển sang máy tính khác hoặc người dùng khác. | Cao: Phụ thuộc vào cấu trúc thư mục nội bộ của dự án, có thể di chuyển và chạy mượt mà trên bất kỳ máy tính hoặc ổ đĩa nào. |
| Độ dài câu lệnh | Thường rất dài và phức tạp, dễ gây sai sót khi gõ hoặc thay đổi cấu trúc. | Ngắn gọn, súc tích và dễ quản lý. |
| Tính an toàn | Rất thấp trong môi trường làm việc nhóm hoặc khi chia sẻ mã nguồn. | Cao, đảm bảo tính đồng bộ khi đóng gói toàn bộ thư mục dự án gửi cho bạn bè. |

## Phần 2: Lựa chọn tối ưu và Ý nghĩa ký hiệu

* Giải pháp tối ưu cho An: Lựa chọn Cách 2 (đường dẫn tương đối) kết hợp với cấu trúc thư mục chuẩn của dự án để đảm bảo hệ thống chạy tốt trên mọi máy tính của bạn bè.  
* Ý nghĩa các ký hiệu:  
  * Ký hiệu . (dấu chấm đơn): Đại diện cho thư mục hiện tại (current directory) nơi file script đang được thực thi.  
  * Ký hiệu .. (hai dấu chấm): Đại diện cho thư mục cấp trên (parent directory) \- di chuyển lùi ra ngoài một bậc từ thư mục hiện tại để tìm đến các thư mục dữ liệu lân cận.

