# Moomi Cloud Drive 1.0.2

Build **37** bổ sung Nhập ảnh, quản lý Phiên bản và cập nhật thư mục khi đang xem trong Finder.

- **Nhập ảnh tự động từ thẻ nhớ, USB và ổ ngoài:** chọn thiết bị đang gắn, thư mục nguồn, tài khoản Google Drive/OneDrive và thư mục cloud đích một lần. Cấu hình mới mặc định bật **Tự nhập khi cắm thiết bị này**; có thể tắt để nhập thủ công.
- Bấm **Kiểm tra ảnh**, xem trước rồi **Bật tự động và nhập ảnh**, hoặc **Lưu cho lần sau**. Những lần cắm lại, app nhập theo cấu hình đã lưu. Thiết bị chưa cấu hình cần thiết lập lần đầu; không tự dùng đích của thiết bị khác.
- App đọc ảnh trong cả thư mục nguồn và các thư mục con, kể cả khi JPEG và RAW nằm lẫn nhau. Ảnh được chia theo ngày chụp EXIF thành thư mục như `08.11.26/Anh Goc` và `08.11.26/Raw`; giữ nguyên file trên thiết bị. RAW có thể dùng ngày của JPEG cùng cặp; ảnh thiếu ngày, cặp không xác định và loại bỏ qua được liệt kê để kiểm tra.
- Nhập ảnh dùng chung giới hạn truyền của tài khoản với Finder. Tiến độ và biên nhận được giữ để tiếp tục; file trùng tên khác nội dung có tên riêng. Giới hạn phần đệm và dừng có kiểm soát khi gặp lỗi, giữ nguồn cùng dữ liệu chưa được xác nhận.
- **Phiên bản:** khi máy này và cloud cùng sửa một file, mặc định giữ riêng bản máy này trước khi nhận bản mới từ cloud. Xem tên, thời gian, dung lượng và mở vị trí lưu trong mục Phiên bản. Bản giữ lại nằm trên máy, không tự tải lên hoặc tự xóa.
- Chọn **Dùng bản máy này**, **Dùng bản cloud** hoặc **Giữ cả hai**. Thay nội dung file Google Drive cần xác nhận và kiểm tra lại phiên bản; nếu cloud có thay đổi mới, app dừng để xem lại. Giữ cả hai tạo thêm file có tên riêng; bản dự phòng vẫn được giữ.
- Thêm các lựa chọn Phiên bản vào **menu chuột phải Finder** cho file và thư mục có bản giữ lại. Thao tác thư mục hiển thị danh sách trước khi áp dụng; file đã đổi phiên bản hoặc ra khỏi phạm vi được báo riêng.
- **Tự cập nhật thư mục đang xem**, mặc định mỗi 3 giây; có thể đổi 3/5/10/30 giây hoặc tắt tại Cài đặt → Finder. Dừng kiểm tra định kỳ khi không dùng Finder/Moomi, máy nghỉ hoặc không có thư mục đang xem. Không quét toàn bộ ổ.
- Sửa danh sách cũ trong bảng chọn thư mục cloud. Kiểm tra lại thư mục đang mở khi chọn đích, và tiếp tục kiểm tra các thư mục Finder còn đang xem sau khi app khởi động lại.
- Sửa cảnh báo phiên bản giả khi nội dung đã lên cloud nhưng bước đổi tên/di chuyển bị mất phản hồi. Giữ việc xác minh nội dung, danh tính file và phiên bản trước khi xác nhận thành công.
- Giảm truy vấn và ghi dữ liệu lặp khi duyệt thư mục; chuyển lưu nhật ký và quét bản sửa khỏi luồng giao diện. Sửa xử lý kết quả đến muộn sau khi hủy và giữ đích tải OneDrive cũ khi lượt tải bị hủy.

Chu kỳ 3 giây là khoảng kiểm tra, không bảo đảm mọi thay đổi hiển thị trong đúng 3 giây. File chưa lưu trong ứng dụng chỉnh sửa chưa thể đồng bộ. Tốc độ thực tế phụ thuộc đường truyền, thiết bị và dịch vụ cloud.

Giữ nguyên helper Keychain v1 đã ký, tài khoản, quyền Finder, cấu hình truyền và tự mount. **OneDrive hiện chỉ upload file mới; thay nội dung file có sẵn chưa được hỗ trợ.** macOS 15+, gói universal Apple Silicon/Intel. Bản hiện tại dùng chứng chỉ nội bộ, chưa có Apple Developer ID/notarization.
