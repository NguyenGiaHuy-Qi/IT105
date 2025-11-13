**Use Case Diagram:**


![Ex1](/Session06/assets/Ex1-SS6.jpg)


## Mô tả các use case chính:

### Use Case 1: Đặt chỗ


| **Thành phần**           | **Nội dung**                                                                                                                                                                       |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tên use case         | Đặt chỗ                                                                                                                                                                            |
| Mô tả ngắn gọn       | Người dùng chọn phim, ngày và giờ chiếu để tiến hành đặt vé xem phim                                                                                                               |
| Actor                | Người dùng                                                                                                                                                                         |
| Điều kiện tiên quyết | Người dùng đã đăng nhập (hoặc truy cập ứng dụng ở màn hình danh sách phim)                                                                                                         |
| Luồng sự kiện chính  | 1. Người dùng chọn bộ phim muốn xem <br>2. Hệ thống hiển thị các suất chiếu theo ngày và rạp <br>3. Người dùng chọn suất chiếu mong muốn <br>4. Hệ thống chuyển sang bước chọn ghế |
| Luồng phụ / Ngoại lệ | Nếu suất chiếu đã hết chỗ -> Hệ thống thông báo và gợi ý suất chiếu khác                                                                                                           |
| Kết quả              | Hệ thống lưu thông tin đặt chỗ tạm thời và chuyển sang bước chọn ghế                                                                                                               |


### Use Case 2: Chọn ghế


| **Thành phần**           | **Nội dung**                                                                                                                                                        |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Tên use case**         | Chọn ghế                                                                                                                                                            |
| **Mô tả ngắn gọn**       | Người dùng chọn vị trí ghế ngồi trong rạp cho suất chiếu đã chọn                                                                                                    |
| **Actor**                | Người dùng                                                                                                                                                          |
| **Điều kiện tiên quyết** | Người dùng đã chọn phim và suất chiếu hợp lệ                                                                                                                        |
| **Luồng sự kiện chính**  | 1. Hệ thống hiển thị sơ đồ ghế của rạp <br>2. Người dùng chọn ghế mong muốn <br>3. Hệ thống kiểm tra tình trạng ghế <br>4. Hệ thống giữ ghế tạm thời cho người dùng |
| **Luồng phụ / Ngoại lệ** | Nếu ghế đã có người khác chọn trước -> Hệ thống thông báo và yêu cầu chọn lại                                                                                       |
| **Kết quả**              | Ghế được giữ thành công và sẵn sàng cho bước thanh toán                                                                                                             |



### Use Case 3: Thanh toán

| **Thành phần**           | **Nội dung**                                                                                                                                                                                                                        |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Tên use case**         | Thanh toán                                                                                                                                                                                                                          |
| **Mô tả ngắn gọn**       | Người dùng tiến hành thanh toán vé đã chọn qua cổng thanh toán điện tử                                                                                                                                                              |
| **Actor**                | Người dùng, Hệ thống thanh toán                                                                                                                                                                                                     |
| **Điều kiện tiên quyết** | Người dùng đã chọn ghế và xác nhận đặt vé                                                                                                                                                                                           |
| **Luồng sự kiện chính**  | 1. Người dùng chọn phương thức thanh toán (thẻ, ví điện tử, ngân hàng, v.v.) <br>2. Hệ thống gửi yêu cầu đến cổng thanh toán <br>3. Hệ thống thanh toán xác nhận giao dịch thành công <br>4. Hệ thống gửi vé điện tử cho người dùng |
| **Luồng phụ / Ngoại lệ** | Nếu thanh toán thất bại → Hệ thống thông báo lỗi và cho phép thử lại hoặc hủy giao dịch                                                                                                                                             |
| **Kết quả**              | Thanh toán thành công, người dùng nhận vé điện tử                                                                                                                                                                                   |


### Use Case 4: Hủy vé


| **Thành phần**           | **Nội dung**                                                                                                                                                     |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Tên use case**         | Hủy vé                                                                                                                                                           |
| **Mô tả ngắn gọn**       | Người dùng hủy vé đã đặt trong thời gian quy định                                                                                                                |
| **Actor**                | Người dùng                                                                                                                                                       |
| **Điều kiện tiên quyết** | Người dùng đã có vé hợp lệ trong lịch sử đặt vé                                                                                                                  |
| **Luồng sự kiện chính**  | 1. Người dùng mở lịch sử đặt vé <br>2. Chọn vé muốn hủy <br>3. Hệ thống kiểm tra thời hạn hủy <br>4. Nếu hợp lệ, hệ thống thực hiện hủy vé và hoàn tiền (nếu có) |
| **Luồng phụ / Ngoại lệ** | Nếu quá hạn hủy → Hệ thống thông báo không thể hủy vé                                                                                                            |
| **Kết quả**              | Vé bị hủy, tiền hoàn trả (toàn phần hoặc một phần) tùy theo quy định                                                                                             |
