## Mối quan hệ giữa các Use Case:


| Use Case A        | Use Case B        | Mối quan hệ              | Giải thích                                                                                                                                                         |
| ----------------- | ----------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Đặt hàng          | Kiểm tra giỏ hàng | Include                  | Khi người dùng thực hiện đặt hàng, hệ thống bắt buộc kiểm tra giỏ hàng để xác nhận sản phẩm, số lượng và tính hợp lệ trước khi tạo đơn hàng.                       |
| Đặt hàng          | Đề xuất hoá đơn   | Include                  | Trong quá trình đặt hàng, hệ thống tự động đề xuất hóa đơn (bao gồm tổng tiền, thuế, phí vận chuyển, giảm giá nếu có) để khách hàng xác nhận trước khi thanh toán. |
| Kiểm tra giỏ hàng | Xem đánh giá      | Extend                   | Khi người dùng kiểm tra sản phẩm trong giỏ, họ có thể mở rộng thao tác để xem đánh giá của sản phẩm nhằm quyết định có mua hay không. Đây là hành vi tùy chọn.     |
| Xem đánh giá      | —                 | Association (Khách hàng) | Khách hàng có thể trực tiếp xem đánh giá sản phẩm mà không cần đặt hàng. Đây là mối quan hệ tác nhân – Use Case thông thường.                                      |
