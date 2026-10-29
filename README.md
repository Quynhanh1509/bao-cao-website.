# Website báo cáo — Pastel hồng & xanh

## Các tệp mã nguồn
- `index.html`: khung trang và cấu hình bảo mật trình duyệt.
- `styles.css`: giao diện pastel hồng/xanh.
- `app.js`: đăng nhập, tải báo cáo và điều hướng.
- `config.js`: URL Supabase và publishable key.
- `utils.js`: hàm tiện ích hiển thị dữ liệu.

## Triển khai
1. Tải các tệp lên thư mục gốc của GitHub repository (cùng cấp với nhau).
2. Bật GitHub Pages từ nhánh `main`, thư mục `/(root)`.
3. Trong Supabase Authentication, cấu hình Site URL và Redirect URLs cho đúng URL GitHub Pages của bạn.
4. Chạy SQL khởi tạo hệ thống trước khi chạy SQL thêm báo cáo mẫu.

## Lưu ý
- `config.js` chứa publishable key, loại khóa này có thể nằm trong frontend. Không bao giờ đặt `service_role` hoặc secret key ở đây.
- Cần cấu hình RLS đúng trên Supabase; không coi giao diện đăng nhập là cơ chế bảo mật duy nhất.
- Website này dùng Supabase JS qua `https://esm.sh/@supabase/supabase-js@2`, nên trình duyệt cần truy cập được miền `esm.sh`.
