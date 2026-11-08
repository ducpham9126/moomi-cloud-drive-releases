# Moomi Cloud Drive

Ứng dụng macOS để sử dụng Google Drive trong Finder, tải theo nhu cầu và truyền tệp trực tiếp lên cloud.

## Cài đặt

[Tải bản mới nhất](https://github.com/ducpham9126/moomi-cloud-drive-releases/releases/latest). Chọn tệp `.dmg`, mở và kéo **Moomi Cloud Drive.app** vào **Applications**. Yêu cầu macOS 15 trở lên; hỗ trợ Apple Silicon và Intel.

Bản hiện tại sử dụng chứng chỉ ký nội bộ, **chưa có Developer ID/notarization của Apple**. Việc mở trên máy Mac khác có thể cần xử lý xác nhận của macOS. Không có yêu cầu tắt Gatekeeper toàn hệ thống.

## Sử dụng

- Đăng nhập Google Drive và mở ổ trong thanh bên Finder.
- Tài khoản được ghim tự động bằng tên ngắn trong Mục ưa thích. Có thể hiện thêm ổ native trong Cài đặt Finder của app.
- Mặc định mở cùng macOS và tự kết nối các tài khoản khi mở app; có thể tắt trong Cài đặt hoặc cho từng tài khoản.
- App mặc định chỉ hiện trên thanh menu. Trong **Cài đặt → Chung → Hiển thị ứng dụng**, có thể hiện/ẩn riêng biểu tượng thanh menu và Dock; lựa chọn được lưu lại. Nếu ẩn cả hai, mở app từ Applications hoặc Spotlight để truy cập lại.
- Giữ ứng dụng chạy để sử dụng ổ cloud; đóng cửa sổ vẫn giữ các kết nối hoạt động.
- Thư mục được kiểm tra thay đổi khi sử dụng Finder. Thời gian hiển thị phụ thuộc callback/bộ nhớ đệm của macOS và phản hồi từ dịch vụ cloud.
- Trong menu ứng dụng chọn **Kiểm tra bản cập nhật…**. Cài đặt có tùy chọn kiểm tra tự động và tải cập nhật tự động. App chờ tác vụ đang chạy trước khi cài cập nhật.

## Phạm vi hiện tại

Google Drive là luồng đã được kiểm thử thực tế. OneDrive cần cấu hình Microsoft App Registration và kiểm thử tài khoản trước khi sử dụng; chưa được xác nhận tương đương Google Drive. Chưa có bản Windows.

Kho này chỉ chứa bản cài, ghi chú phát hành và dữ liệu cập nhật có chữ ký. Mã nguồn được lưu ở kho riêng tư của chủ sở hữu. Token tài khoản và khóa ký không nằm trong kho này.
