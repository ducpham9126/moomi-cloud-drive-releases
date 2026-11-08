# Moomi Cloud Drive 1.0.1

Build **36** sửa luồng cho phép ổ cloud khi cài lần đầu trên máy Mac khác.

- Sửa hướng dẫn sai dẫn người dùng đến mục Mở khi đăng nhập/phần mở rộng macOS. File Provider đã có sẵn trong app; quyền bật ổ native được macOS hỏi trong Finder.
- Sau khi đăng nhập hoặc chủ động kết nối, app tự mở đúng ổ đang chờ quyền để người dùng bấm xác nhận của macOS. Khởi động tự động không bật hàng loạt cửa sổ hướng dẫn. Nút **Cho phép trong Finder…** vẫn có để mở lại khi cần. Menu tài khoản trên thanh menu cũng dùng cùng thao tác. App chỉ mở giao diện xin quyền của macOS; người dùng tự chọn Bật/Cho phép.
- Nhận sự kiện thay đổi domain của macOS khi app hoặc Finder đang được sử dụng, đồng thời kiểm tra lại khi quay về app. Kiểm tra các tài khoản đang chờ quyền, kể cả tài khoản không được chọn. Sau lần bật đầu tiên, hoàn tất lối tắt tên ngắn, dung lượng và tùy chọn tự mở Finder.
- Không lặp đăng ký hoặc thiết lập thanh bên khi nhận nhiều sự kiện quay lại. Kết quả đến muộn không được tự kết nối lại tài khoản mà người dùng đã ngắt.
- Giữ dịch vụ Keychain v1 đã ký, các tài khoản và cài đặt. Không thay cơ chế truyền tệp hay chạy phép đo tốc độ trong bản sửa này.

Kiểm thử chuyển trạng thái dùng dữ liệu giả, không tự bật/tắt quyền hệ thống. Luồng cài lần đầu trên máy Mac khác cần chủ máy xác nhận trong Finder; kiểm thử trên máy phát triển đã bật quyền không thay thế bước đó.

macOS 15+, gói universal Apple Silicon/Intel. OneDrive hỗ trợ upload file mới; khi sửa nội dung file có sẵn, lưu thành bản mới. Bản hiện tại chưa có Apple Developer ID/notarization. Bản chính thức đầu tiên 1.0.0/build35 và các bản thử trước đó được giữ nguyên.
