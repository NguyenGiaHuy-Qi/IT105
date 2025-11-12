1. Khách hàng (User)

- Vai trò: Là tác nhân bên ngoài (actor) khởi tạo các tương tác trong hệ thống.

- Chức năng:

    + Truy cập vào Website để xem sản phẩm, chọn hàng, đặt hàng.

    + Cung cấp thông tin cần thiết (ví dụ: địa chỉ giao hàng, thông tin thanh toán).

    + Xác nhận và thực hiện thanh toán.

    + Nhận phản hồi từ hệ thống (thông báo thanh toán thành công, đơn hàng được xác nhận...).

2. Website (Ứng dụng web)

- Vai trò: Là trung gian xử lý nghiệp vụ chính, kết nối giữa Khách hàng và Hệ thống thanh toán.

- Chức năng:

    + Nhận yêu cầu từ khách hàng (xem sản phẩm, đặt hàng, yêu cầu thanh toán).

    + Kiểm tra dữ liệu đầu vào (số lượng hàng, thông tin giao hàng...).

    + Gửi yêu cầu thanh toán đến Hệ thống thanh toán.

    + Nhận phản hồi kết quả thanh toán (thành công / thất bại).

    + Thông báo kết quả giao dịch lại cho Khách hàng.

3. Hệ thống thanh toán (Payment Gateway / Payment System)

- Vai trò: Là bên thứ ba chuyên xử lý các giao dịch tài chính.

- Chức năng / nhiệm vụ:

    + Nhận yêu cầu thanh toán từ Website (bao gồm thông tin giao dịch, số tiền, phương thức thanh toán...).

    + Xác thực thông tin thẻ / tài khoản ngân hàng của Khách hàng.

    + Thực hiện xử lý thanh toán (ghi nợ, chuyển tiền...).

    + Gửi phản hồi kết quả (thành công / thất bại / lỗi) về cho Website.