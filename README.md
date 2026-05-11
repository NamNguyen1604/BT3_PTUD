
# Lớp: 58KTPM
# MSSV : K225480106092
# Bài tập 03:
# SỬ DỤNG WORDPRESS ĐỂ TẠO WEB SITE
1 Mục tiêu bài tập
- Sử dụng Docker Compose để thiết lập hệ thống mã nguồn mở WordPress, quản trị qua PhpMyAdmin và public ra internet bằng Cloudflare Tunnel.
2. Cấu trúc hệ thống (Docker Compose)
  Hệ thống bao gồm 3 dịch vụ chính:
- MariaDB (Latest):** Quản trị cơ sở dữ liệu.
- PhpMyAdmin (Latest):** Quản lý DB trực quan qua web (Port 8081).
- WordPress (Latest):** CMS chính để xây dựng nội dung (Port 8001).
# Deadline : 23h59 ngày 12 tháng 5 năm 2026.
## BÀI LÀM 
1.Tạo 1 dự án chứa bài tập:
- Sử dụng lệnh : mkdir ~/wordpress_project && cd ~/wordpress_project
<img width="643" height="56" alt="image" src="https://github.com/user-attachments/assets/2a59f9f7-e3f0-4176-870f-758d80daa9fe" />
<img width="752" height="764" alt="image" src="https://github.com/user-attachments/assets/044cb02b-3e93-49f6-bf23-f83987f481e8" />
- tạo file cấu hình docer-compose.yml và khởi động hệ thống
2.Sửa cấu hình Cloudflare Tunnel
 <img width="551" height="28" alt="image" src="https://github.com/user-attachments/assets/c753a214-0991-49b3-af5a-77a19df3d60f" />
 <img width="962" height="1080" alt="image" src="https://github.com/user-attachments/assets/885c8246-85e8-4568-a625-0af5fcfa6eb4" />
3.Tạo bản ghi DNS mới và Chạy Tunnel và vào web
<img width="1326" height="116" alt="image" src="https://github.com/user-attachments/assets/df46b745-c6a2-4e16-9263-eb9cb5319124" />
4.Thiết lập WordPress
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b3b096f3-e308-4065-baeb-cfaf5700ca00" />
5.Thêm bài viết
  5.1. Tạo 1 bài viết trong wordpress giới thiệu về bản thân sinh viên: thông tin cá nhân, sở thích, ... bài viết có thể chứa hình ảnh, âm thanh, video, ...
  <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/03ec37fb-d6e6-4575-85bd-50b5986c9c5f" />
  5.2 Tạo 1 bài viết trong wordpress giới thiệu về ngành học mà em yêu thích trong trường TNUT. bài viết phải chứa hình ảnh, video, ...
  <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7cc98189-1c6c-4e53-b5ae-641315165c30" />
# Nhận xét về việc sử dụng WordPress
- Tính khả dụng:WordPress cực kỳ dễ dùng với giao diện kéo thả, giúp sinh viên IT nhanh chóng có một sản phẩm web hoàn chỉnh mà không tốn quá nhiều công sức code backend.
- Độ khó: Việc cấu hình qua Docker đòi hỏi kiến thức về mạng và hệ điều hành Linux, nhưng một khi đã chạy thì việc quản trị nội dung rất đơn giản.
- Tài nguyên hệ thống: Sử dụng Docker giúp tối ưu hóa tài nguyên máy chủ.
    WordPress tiêu tốn khoảng 300-500MB RAM, hoàn toàn phù hợp để chạy trên các máy ảo VPS phổ thông.
    Việc sử dụng Cloudflare Tunnel giúp bảo mật server vì không cần mở port trên Router/Firewall của máy thật.




