### Sơ đồ kiến trúc tổng thể

![Ex6](/Session07/assets/Ex6-SS7.jpg)


### Mô tả luồng hoạt động nghiệp vụ chính

Luồng: Khách hàng mua hàng và thanh toán online

1. Khách hàng chọn sản phẩm → thêm vào giỏ hàng → nhấn “Thanh toán”.
2. Frontend gửi yêu cầu thanh toán đến Backend API.
Order Management Module tạo đơn hàng ở trạng thái "Pending".
3. Payment Module gọi VNPay API → chuyển người dùng đến trang thanh toán VNPay.
4. VNPay xử lý giao dịch → trả callback xác nhận cho Backend.
5. Backend cập nhật đơn hàng sang "Paid" và trừ tồn kho trong Inventory Module.
6. Email Notification Module gửi email xác nhận đơn hàng qua SMTP Server.
7. Frontend hiển thị kết quả thanh toán thành công cho người dùng.