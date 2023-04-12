ĐỀ TÀI: XÂY DỰNG CHƯƠNG TRÌNH CHAT

Yêu cầu về chức năng phía client (phải có GUI):
▪ Đăng ký tài khoản mới, đăng nhập, cập nhật thông tin tài khoản. Thông tin tối thiểu cho mỗi
tài khoản gồm có các trường: username (chính là địa chỉ email), password (hash), họ tên, giới
tính, ngày sinh. Ngoài ra, địa chỉ email lúc đăng ký phải được xác thực bằng OTP (timeout 10
phút) trước khi tài khoản đó được kích hoạt.
▪ Tạo nhóm chat mới hoặc gia nhập/rời khỏi các nhóm chat có sẵn.
▪ Gửi tin nhắn 1-1 hoặc 1-nhóm.
▪ Gửi file đính kèm (dung lượng dưới 1MB), gửi sticker.
▪ Chặn nhận tin nhắn từ 1 người dùng hoặc 1 nhóm.
▪ Xác nhận tin nhắn đã gửi/nhận, đã xem.
▪ Friend list: lưu giữ danh sách và cho biết trạng thái (online hoặc offline) của những người mà user
đã từng chat, có thông báo khi bất cứ user nào trong friend list thay đổi trạng thái.
▪ Chức năng quản lý và lưu giữ tin nhắn: toàn bộ tin nhắn của người dùng được lưu trữ trên
server, khi client đăng nhập, những tin nhắn gần đây nhất sẽ được đẩy về giao diện phía client.

Yêu cầu về chức năng phía server (không cần GUI):
▪ Thống kê được tổng số user, các user đang online.
▪ Ghi log khi user login/logout hoặc thực hiện các chức năng: đăng ký tài khoản; tạo nhóm.
▪ Block user bằng lệnh (hoặc giao diện đồ họa nếu có).
▪ Broadcast tin nhắn từ hệ thống đến toàn bộ user.

Yêu cầu chung:
▪ Mã hóa nội dung tin nhắn giữa client – server. Phải sử dụng key khác nhau cho các client.
▪ Các client khi chấm bài phải chạy trên các máy tính khác nhau.
