# Moomi Cloud Drive

Ứng dụng macOS để sử dụng Google Drive và OneDrive trong Finder, tải theo nhu cầu và truyền tệp trực tiếp lên cloud.

## Cài đặt

[Tải bản mới nhất](https://github.com/ducpham9126/moomi-cloud-drive-releases/releases/latest). Chọn tệp `.dmg`, mở và kéo **Moomi Cloud Drive.app** vào **Applications**. Yêu cầu macOS 15 trở lên; hỗ trợ Apple Silicon và Intel.

Ghi chú phát hành chính thức: [1.0.0 · build 29](RELEASE-1.0.0-build29.md) — tag `v1.0.0-build29`.

Bản hiện tại sử dụng chứng chỉ ký nội bộ, **chưa có Developer ID/notarization của Apple**. Việc mở trên máy Mac khác có thể cần xử lý xác nhận của macOS. Không có yêu cầu tắt Gatekeeper toàn hệ thống.

## Sử dụng

- Chọn Google Drive hoặc OneDrive, đăng nhập và mở ổ trong thanh bên Finder; không nhập Application ID hoặc cấu hình Azure trong app.
- Tài khoản được ghim tự động bằng tên ngắn trong Mục ưa thích. Có thể hiện thêm ổ native trong Cài đặt Finder của app.
- Mặc định mở cùng macOS và tự kết nối các tài khoản khi mở app; có thể tắt trong Cài đặt hoặc cho từng tài khoản.
- App mặc định chỉ hiện trên thanh menu. Trong **Cài đặt → Chung → Hiển thị ứng dụng**, có thể hiện/ẩn riêng biểu tượng thanh menu và Dock; lựa chọn được lưu lại. Nếu ẩn cả hai, mở app từ Applications hoặc Spotlight để truy cập lại.
- Giữ ứng dụng chạy để sử dụng ổ cloud; đóng cửa sổ vẫn giữ các kết nối hoạt động.
- Thư mục được kiểm tra thay đổi khi sử dụng Finder. Thời gian hiển thị phụ thuộc callback/bộ nhớ đệm của macOS và phản hồi từ dịch vụ cloud.
- Trong menu ứng dụng chọn **Kiểm tra bản cập nhật…**. Cài đặt có tùy chọn kiểm tra tự động và tải cập nhật tự động. App chờ tác vụ đang chạy trước khi cài cập nhật.

## Phạm vi hiện tại

Google Drive là luồng đã được kiểm thử thực tế. OneDrive bổ sung đăng nhập Microsoft, đọc/tải file, tạo thư mục, upload file mới, đổi tên, di chuyển và chuyển vào Thùng rác. **Ghi đè nội dung OneDrive chưa được hỗ trợ; khi chỉnh sửa file có sẵn, hãy lưu thành bản mới.** Tài khoản tổ chức có thể cần quản trị viên cho phép ứng dụng. Chưa có bản Windows.

Kho này chỉ chứa bản cài, ghi chú phát hành và dữ liệu cập nhật có chữ ký. Mã nguồn được lưu ở kho riêng tư của chủ sở hữu. Token tài khoản và khóa ký không nằm trong kho này.
