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


## Giao diện mới
Phiên bản này cân bằng giữa sự chuyên nghiệp và nét đáng yêu: nền sáng, hồng pastel và xanh lavender tiết chế, thẻ bo góc vừa phải, điểm nhấn nhẹ, bố cục rõ ràng và vẫn giữ nguyên luồng ứng dụng hiện có.

## Cập nhật GitHub Pages
Giải nén ZIP và tải nội dung bên trong thư mục `bao-cao-website-cute-professional` lên đúng repository đang dùng cho GitHub Pages (giữ `index.html` ở thư mục gốc của repository). Sau khi commit/push, đợi GitHub Pages triển khai xong rồi tải lại mạnh trang bằng `Command + Shift + R` trên Mac. Không thay `config.js`/thiết lập Supabase bằng thông tin khác nếu website đang kết nối cơ sở dữ liệu hiện tại.
