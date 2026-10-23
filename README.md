# AI Live Studio

Bộ project AI Live Studio được tổng hợp từ các gói cập nhật và hai bản final 1.0.0: AI Live Studio Customer và AI Live Admin Bot. Repo gồm mã nguồn có thể đọc, test, tài liệu từng giai đoạn và nhật ký phát triển.

> Repo giữ mã nguồn và tài liệu. Bộ cài `.exe`, runtime nhúng và cấu hình riêng không được đưa vào; các gói phát hành gốc vẫn được giữ riêng trong Library.

## Cấu trúc

- `source/1.0.0/customer/` — mã nguồn, giao diện và tài liệu từ bản final khách hàng 1.0.0.
- `source/1.0.0/admin-bot/` — mã Cloudflare/admin, bài test và hướng dẫn từ bản final Admin Bot 1.0.0.
- `source/0.9.6/` — mã nguồn nền Windows 0.9.6 để đối chiếu với các bản nâng cấp sau đó.
- `history/patches/` — mã và hướng dẫn của các cập nhật/bugfix trước 1.0.0, chia theo tên gói.
- `history/releases/` — mã nguồn/tài liệu trích từ các snapshot Windows 0.9.5, 0.9.5.2 và 0.9.5.3.
- `releases/0.9.7/docs/` — tài liệu/script văn bản của bản phát hành 0.9.7; file thực thi đã loại khỏi repo.
- `DEVELOPMENT_HISTORY.md` — các mốc phát triển dựa trên ghi chú đi kèm từng gói.
- `SOURCES.md` — danh sách gói nguồn và SHA-256 của hai gói final 1.0.0.

## Các phần chính

- Ứng dụng điều phối livestream với OBS, video, sản phẩm và tương tác.
- Dịch vụ cấp phép và công cụ quản trị.
- Bot Telegram và tiện ích đọc bình luận.
- Kết nối Shopee, hỗ trợ livestream nhiều shop và các bản sửa lỗi OBS.

## Bắt đầu xem mã

1. Đọc `DEVELOPMENT_HISTORY.md` để nắm thứ tự các mốc.
2. Bắt đầu với bản final ở `source/1.0.0/`.
3. Đối chiếu các bản vá trước đó trong `history/patches/`.
4. Xem hướng dẫn tại `HUONG-DAN*`, `README*` và ghi chú QA của từng bản.

Các gói cập nhật cũ thường chỉ chứa những tệp cần thay thế; chúng không phải bản cài độc lập. Bản 0.9.6 được giữ để đối chiếu lịch sử, không thay thế bản final 1.0.0.

## Bảo mật

Không đưa token Telegram, Shopee Partner Key, khóa ký riêng, khóa phát livestream, `settings.json`, `.env` có giá trị thật, secrets Cloudflare, dữ liệu khách hàng hoặc dump D1 lên repo công khai. Dùng biến môi trường và giá trị giả cho kiểm thử. Repo này đã loại cấu hình `settings.json`, runtime nhúng và file thực thi.

Chưa triển khai lại các mã nguồn này lên tài khoản Shopee, Telegram, OBS hoặc Cloudflare. Hãy rà soát secrets và quyền truy cập trước khi chạy hoặc triển khai.

## Giấy phép

Các gói nguồn không cung cấp một giấy phép chung cho toàn bộ project. Repo chưa tự gán giấy phép tái sử dụng. Hãy xác nhận quyền sở hữu và điều kiện của thư viện bên thứ ba trước khi phân phối lại.
