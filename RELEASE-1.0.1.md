# Moomi Cloud Drive 1.0.1

Build **23** bổ sung đo và chọn số lượt upload Google Drive theo từng tài khoản.

- Có lối tắt Finder mang tên ngắn của tài khoản, tạo tại **Cài đặt → Finder → Tạo lối tắt tên ngắn…**. Người dùng kéo alias vào Mục ưa thích một lần; alias có biểu tượng cloud, giữ identity khi đổi tên và tránh ghi đè lối tắt của tài khoản khác.
- Sau khi đã ghim và kiểm tra lối tắt, có thể ẩn tên ổ dài trong Vị trí qua tùy chọn có xác nhận. Có thể bật lại; thay đổi này giữ nguyên domain, kết nối và file cloud.
- Có lựa chọn **Tự động** sử dụng mức upload phù hợp từ kết quả đo của chính tài khoản đang chọn. Mức thủ công đã đặt được giữ nguyên; app không tự chuyển các tài khoản hiện có sang Tự động.
- Phép đo thử các mức 1–8 hai lượt theo thứ tự ngược nhau, sau đó kiểm tra lại hai mức tốt nhất. File QA được xác minh nội dung bằng MD5; chỉ kết quả hợp lệ mới được dùng để chọn mức Tự động.
- Phép đo chỉ bắt đầu khi người dùng chủ động xác nhận, upload dự kiến khoảng **2,3 GiB**, chưa tính metadata hoặc thử lại. Dữ liệu thử nằm trong thư mục QA riêng, được giữ lại để kiểm tra; không dùng file công việc và không tự chạy phép đo ở nền. Dữ liệu thử và báo cáo cũng dùng dung lượng trên máy.
- Kết quả phụ thuộc mạng và dịch vụ cloud tại thời điểm đo; không phải cam kết đạt cùng tốc độ trên mọi mạng. Có thể đo lại khi điều kiện thay đổi.
- Sửa trường hợp phản hồi đọc thư mục cũ đến muộn sau một thay đổi mới, làm danh sách Finder lùi về trạng thái cũ. Phản hồi cũ được bỏ và thư mục được kiểm tra lại.
- Dọn đúng file tải tạm nếu bước xác minh phiên bản thất bại hoặc bị hủy sau khi tải. Finder chỉ nhận nội dung sau khi kiểm tra cuối hoàn tất.

Vẫn hỗ trợ macOS 15 trở lên, gói universal Apple Silicon/Intel. OneDrive vẫn cần cấu hình và kiểm thử tài khoản thật; ghi đè nội dung OneDrive chưa được bật. Bản hiện tại chưa có Apple Developer ID/notarization.

Bản 1.0.0/build22 đã phát hành được giữ nguyên. Bản 1.0.1 dùng build mới và cơ chế cập nhật có chữ ký sẵn có; tài khoản, lựa chọn tự kết nối và cấu hình thủ công được giữ qua cập nhật.
