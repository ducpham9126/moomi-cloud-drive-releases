# Moomi Cloud Drive 1.0.2

Build **37** cải thiện độ mới của dữ liệu Finder và giảm công việc làm chậm giao diện.

- Khi xem thư mục, kiểm tra lại tên, vị trí, quyền và sự tồn tại của chính thư mục đó, kể cả khi thư mục cha không nằm trong lượt làm mới. Không coi thư mục đã xóa trên cloud là một thư mục trống còn tồn tại.
- Ngăn thông tin file cũ hoặc kết quả đến sau khi hủy ghi đè dữ liệu mới trong Finder. Giữ việc kiểm tra phiên bản và toàn vẹn nội dung trước khi giao file cho macOS.
- Cho lượt duyệt thông thường dùng chung truy vấn thư mục mới đang chạy. Yêu cầu làm mới chủ động vẫn khởi tạo truy vấn mới nếu truy vấn cũ đã bắt đầu trước đó; không thêm bộ nhớ đệm theo thời gian.
- Nút Mở trong Finder chỉ chờ kiểm tra thư mục gốc cần mở, tránh phải chờ các thư mục đã xem trước đó. Khi các yêu cầu được gộp, vẫn giữ đầy đủ phạm vi cần làm mới.
- Tái sử dụng bộ phân tích ngày giờ với khóa bảo vệ khi đọc song song, giữ nguyên kết quả và độ chính xác. Đo CPU với 2.000 thời điểm hỗn hợp cho kết quả khoảng 0,12 giây so với 0,50 giây trước sửa; đây không phải số đo băng thông.
- Chuyển ghi nhật ký và quét các bản sửa cần khôi phục khỏi luồng giao diện. Gộp ghi nhật ký theo khoảng ngắn cố định, giữ thứ tự và chờ ghi cuối khi thoát; không để dòng sự kiện liên tục trì hoãn lưu mãi.
- Sửa trường hợp tải OneDrive bị hủy ngay sau phản hồi kiểm tra cuối nhưng vẫn ghi đè đích tải. Khi hủy, giữ đích cũ và dọn bản tải tạm của lượt đó.

Thư mục cloud vẫn được kiểm tra theo thao tác sử dụng. Không thêm vòng quét cloud khi người dùng không thao tác. Tốc độ thực tế phụ thuộc đường truyền, dịch vụ và công việc đang chạy; bản này không cam kết một tốc độ mạng tối đa cố định.

Giữ nguyên dịch vụ Keychain v1 đã ký, tài khoản, quyền Finder, cấu hình truyền, tự mount và giao diện. OneDrive hiện hỗ trợ upload file mới; khi sửa nội dung file có sẵn, lưu thành bản mới. macOS 15+, gói universal Apple Silicon/Intel. Bản hiện tại chưa có Apple Developer ID/notarization.
