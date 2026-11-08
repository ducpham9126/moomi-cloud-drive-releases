# Moomi Cloud Drive

Ứng dụng macOS để sử dụng Google Drive và OneDrive trong Finder, tải theo nhu cầu và truyền tệp trực tiếp lên cloud.

## Cài đặt

[Tải bản mới nhất](https://github.com/ducpham9126/moomi-cloud-drive-releases/releases/latest). Chọn tệp `.dmg`, mở và kéo **Moomi Cloud Drive.app** vào **Applications**. Yêu cầu macOS 15 trở lên; hỗ trợ Apple Silicon và Intel.

Phiên bản hiện đang phát hành nằm tại trang **Latest** phía trên. Bản đầu chính thức [1.0.0 · build 35](RELEASE-1.0.0-build35.md) được giữ nguyên.

Bản hiện tại sử dụng chứng chỉ ký nội bộ, **chưa có Developer ID/notarization của Apple**. Việc mở trên máy Mac khác có thể cần xử lý xác nhận của macOS. Không có yêu cầu tắt Gatekeeper toàn hệ thống.

## Sử dụng

- Chọn Google Drive hoặc OneDrive, đăng nhập và mở ổ trong thanh bên Finder; không nhập Application ID hoặc cấu hình Azure trong app.
- Sau khi đăng nhập, app tự mount. Nếu macOS cần quyền dùng ổ cloud lần đầu, app tự mở đúng ổ trong Finder để bạn bấm **Bật/Cho phép**; không cần tìm Cài đặt hay cài gói mở rộng. App nhận trạng thái từ macOS và kiểm tra lại khi quay về cửa sổ chính. **Mở khi đăng nhập** là tùy chọn khác.
- Tài khoản được ghim tự động bằng tên ngắn trong Mục ưa thích. Có thể hiện thêm ổ native trong Cài đặt Finder của app.
- Mặc định mở cùng macOS và tự kết nối các tài khoản khi mở app; có thể tắt trong Cài đặt hoặc cho từng tài khoản.
- App mặc định chỉ hiện trên thanh menu. Trong **Cài đặt → Chung → Hiển thị ứng dụng**, có thể hiện/ẩn riêng biểu tượng thanh menu và Dock; lựa chọn được lưu lại. Nếu ẩn cả hai, mở app từ Applications hoặc Spotlight để truy cập lại.
- Giữ ứng dụng chạy để sử dụng ổ cloud; đóng cửa sổ vẫn giữ các kết nối hoạt động.
- Đăng nhập được lưu trong Keychain qua helper có danh tính cố định giữa các bản cập nhật app. Khi chuyển từ bản thử cũ có thể cần cấp quyền một lần.
- Thư mục đang xem trong Finder được kiểm tra định kỳ, mặc định mỗi 3 giây; có thể đổi hoặc tắt trong **Cài đặt → Finder**. App dừng kiểm tra định kỳ khi không dùng Finder/Moomi hoặc máy nghỉ. Thời gian hiển thị còn phụ thuộc macOS và phản hồi của dịch vụ cloud.
- Trong **Phiên bản**, xem các bản máy này được giữ lại khi file cùng được sửa trên cloud; chọn **Dùng bản cloud**, **Dùng bản máy này** hoặc **Giữ cả hai**. Bản giữ lại không tự bị xóa. Thao tác thay file Google Drive cần xác nhận và kiểm tra lại phiên bản; OneDrive hiện chỉ tạo file mới. Có thể mở các lựa chọn này từ menu chuột phải Finder của file hoặc thư mục có bản giữ lại.
- Trong **Nhập ảnh**, chọn thư mục nguồn trên thẻ nhớ/USB/ổ ngoài, tài khoản cloud và thư mục đích; xem trước rồi tải lên. Ảnh được xếp theo ngày chụp EXIF vào các thư mục `dd.MM.yy/Anh Goc` và `dd.MM.yy/Raw`, giữ nguyên file nguồn. Có thể bật tự nhập khi cắm đúng thiết bị cho từng cấu hình; lượt chưa xác nhận được giữ để tiếp tục. Ảnh thiếu ngày chụp và cặp RAW/XMP không xác định được liệt kê để kiểm tra.
- Trong menu ứng dụng chọn **Kiểm tra bản cập nhật…**. Cài đặt có tùy chọn kiểm tra tự động và tải cập nhật tự động. App chờ tác vụ đang chạy trước khi cài cập nhật.

## Phạm vi hiện tại

Google Drive là luồng đã được kiểm thử thực tế. OneDrive bổ sung đăng nhập Microsoft, đọc/tải file, tạo thư mục, upload file mới, đổi tên, di chuyển và chuyển vào Thùng rác. **Ghi đè nội dung OneDrive chưa được hỗ trợ; khi chỉnh sửa file có sẵn, hãy lưu thành bản mới.** Tài khoản tổ chức có thể cần quản trị viên cho phép ứng dụng. Chưa có bản Windows.

Kho này chỉ chứa bản cài, ghi chú phát hành và dữ liệu cập nhật có chữ ký. Mã nguồn được lưu ở kho riêng tư của chủ sở hữu. Token tài khoản và khóa ký không nằm trong kho này.
