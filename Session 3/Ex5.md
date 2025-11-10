## BẢNG XÁC ĐỊNH ACTOR, LOẠI VÀ USE CASE PHỤC VỤ:


| **Actor**              | **Loại (Primary / Secondary)** | **Use Case phục vụ**                                                                                                                                                     |
| ---------------------- | ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Khách hàng             | Primary                        | - Đăng ký / Đăng nhập <br> - Tìm kiếm món ăn / nhà hàng <br> - Đặt món <br> - Thanh toán đơn hàng <br> - Theo dõi trạng thái giao hàng <br> - Đánh giá món ăn / nhà hàng |
| Tài xế giao hàng       | Primary                        | - Nhận đơn giao <br> - Xem chi tiết đơn hàng <br> - Cập nhật trạng thái giao hàng (đã nhận / đang giao / đã giao)                                                        |
| Nhà hàng / Quán ăn     | Primary                        | - Quản lý thực đơn <br> - Xác nhận đơn hàng <br> - Cập nhật tình trạng món ăn (hết hàng, còn hàng)                                                                       |
| Quản trị viên hệ thống | Secondary                      | - Quản lý người dùng (khách hàng, tài xế, nhà hàng) <br> - Giám sát và xử lý sự cố hệ thống <br> - Quản lý nội dung và chính sách                                        |
| Hệ thống thanh toán    | Secondary                      | - Xử lý giao dịch thanh toán trực tuyến <br> - Xác nhận trạng thái thanh toán (thành công / thất bại)                                                                    |
| Dịch vụ bản đồ / GPS   | Secondary                      | - Cung cấp vị trí giao hàng và chỉ đường cho tài xế <br> - Tính toán khoảng cách và thời gian giao hàng dự kiến                                                          |
