# Moomi Cloud Drive 1.1.0

Build **28** bổ sung đăng nhập OneDrive bằng ứng dụng Microsoft riêng của Moomi, đăng ký trong **Entra Free**.

- Người dùng chọn OneDrive rồi đăng nhập tài khoản Microsoft; không nhập Application ID hoặc cấu hình Azure trong app.
- Hỗ trợ đọc/tải file, tạo thư mục, tải lên file mới, đổi tên, di chuyển và chuyển vào Thùng rác trên OneDrive. Ghi đè nội dung file có sẵn vẫn bị chặn; khi chỉnh sửa, lưu thành bản mới.
- Kiểm tra tên OneDrive nhất quán trước khi upload, tạo thư mục và đổi tên/di chuyển; giữ tên tiếng Việt, `#` và `%` khi tài khoản cho phép.
- Thêm chẩn đoán API OneDrive với dữ liệu thử trong thư mục QA UUID riêng và đối chiếu bytes/SHA256; không xem đây là kiểm thử Finder hoặc đo tốc độ tối đa.
- Giữ giao diện, tài khoản Google Drive, tự mount, đăng nhập macOS và lựa chọn biểu tượng thanh menu/Dock.

Đăng nhập desktop dùng public client và PKCE, không có Microsoft client secret. Moomi không triển khai máy chủ hay tài nguyên Azure tính phí cho kết nối này. Dung lượng/quyền truy cập vẫn theo tài khoản OneDrive của người dùng; tài khoản tổ chức có thể cần quản trị viên cho phép ứng dụng.

macOS 15+, gói universal Apple Silicon/Intel. Bản hiện tại chưa có Apple Developer ID/notarization.
