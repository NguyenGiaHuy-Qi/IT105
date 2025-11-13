1. Danh sách Stakeholders


| **Stakeholder**                                  | **Vai trò**                                                                        | **Nguồn yêu cầu**                     |
| ------------------------------------------------ | ---------------------------------------------------------------------------------- | ------------------------------------- |
| **Học viên (Student)**                           | Người đăng ký tài khoản, mua khóa học, học online, làm bài kiểm tra, xem kết quả   | Yêu cầu từ người dùng cuối            |
| **Giảng viên (Instructor)**                      | Người tạo, quản lý nội dung khóa học, đăng bài giảng, chấm điểm, phản hồi học viên | Yêu cầu từ người dạy                  |
| **Quản trị viên hệ thống (Admin)**               | Quản lý người dùng, khóa học, giao dịch, xử lý khiếu nại, duy trì hệ thống         | Yêu cầu vận hành hệ thống             |
| **Bộ phận hỗ trợ kỹ thuật (Support Staff)**      | Hỗ trợ kỹ thuật cho người dùng (đăng nhập, lỗi hệ thống, thanh toán)               | Yêu cầu hỗ trợ người dùng             |
| **Nhà quản lý (Manager)**                        | Theo dõi báo cáo doanh thu, thống kê người học, đánh giá chất lượng khóa học       | Yêu cầu quản lý, kinh doanh           |
| **Hệ thống thanh toán (Payment Gateway)**        | Cung cấp dịch vụ xử lý thanh toán cho người mua khóa học                           | Yêu cầu tích hợp từ bên thứ ba        |
| **Nhà cung cấp nội dung (Content Provider)**     | Cung cấp tài liệu, video, đề thi, nội dung giảng dạy                               | Yêu cầu tích hợp nguồn học liệu ngoài |
| **Cơ quan chứng nhận (Certification Authority)** | Cấp chứng chỉ học tập cho học viên hoàn thành khóa học                             | Yêu cầu hợp tác đối tác               |



2. Yêu cầu chức năng (Functional Requirements)


| **Mã yêu cầu** | **Tên chức năng**                         | **Mô tả chi tiết**                                                                                       |
| -------------- | ----------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| **FR1**        | Đăng ký và đăng nhập người dùng           | Học viên và giảng viên có thể tạo tài khoản, đăng nhập, quản lý hồ sơ cá nhân.                           |
| **FR2**        | Quản lý khóa học                          | Giảng viên có thể tạo, chỉnh sửa, xóa khóa học; quản lý bài giảng, video, tài liệu.                      |
| **FR3**        | Mua và thanh toán khóa học                | Học viên có thể chọn khóa học, thanh toán qua ví điện tử, thẻ ngân hàng, PayPal...                       |
| **FR4**        | Quản lý học tập                           | Học viên có thể truy cập nội dung học, theo dõi tiến trình, làm bài tập, kiểm tra, nhận chứng chỉ.       |
| **FR5**        | Tương tác giảng viên – học viên           | Học viên có thể đặt câu hỏi, nhận phản hồi; giảng viên có thể tổ chức diễn đàn hoặc buổi học trực tuyến. |
| **FR6**        | Quản lý bài kiểm tra                      | Tạo, chỉnh sửa, chấm điểm bài kiểm tra, lưu kết quả.                                                     |
| **FR7**        | Quản lý chứng chỉ                         | Cấp chứng chỉ tự động cho học viên hoàn thành khóa học, có thể tải xuống.                                |
| **FR8**        | Quản lý người dùng (Admin)                | Admin có thể khóa/mở tài khoản, phân quyền người dùng.                                                   |
| **FR9**        | Quản lý báo cáo và thống kê               | Thống kê số học viên, doanh thu, khóa học phổ biến, tỷ lệ hoàn thành khóa học.                           |
| **FR10**       | Quản lý phản hồi và hỗ trợ                | Học viên có thể gửi phản hồi; bộ phận hỗ trợ xử lý yêu cầu, theo dõi lịch sử hỗ trợ.                     |
| **FR11**       | Tích hợp thanh toán và xác thực giao dịch | Hệ thống tích hợp API thanh toán để xác nhận giao dịch an toàn.                                          |
| **FR12**       | Gửi thông báo                             | Hệ thống gửi thông báo qua email hoặc ứng dụng khi có khóa học mới, phản hồi, hoặc chứng chỉ.            |



3. Yêu cầu phi chức năng (Non-functional Requirements)


| **Nhóm yêu cầu**                             | **Mã** | **Tên / Nội dung**     | **Mô tả chi tiết**                                                                   |
| -------------------------------------------- | ------ | ---------------------- | ------------------------------------------------------------------------------------ |
| **Hiệu năng (Performance)**                  | NFR1   | Tốc độ phản hồi        | Thời gian phản hồi của hệ thống ≤ 3 giây cho các thao tác cơ bản.                    |
|                                              | NFR2   | Tải đồng thời          | Hệ thống hỗ trợ tối thiểu 10.000 người dùng truy cập đồng thời.                      |
| **Bảo mật (Security)**                       | NFR3   | Xác thực & phân quyền  | Mỗi người dùng đăng nhập bằng tài khoản riêng; dữ liệu phân quyền theo vai trò.      |
|                                              | NFR4   | Mã hóa dữ liệu         | Thông tin thanh toán, mật khẩu được mã hóa (AES-256, HTTPS, JWT).                    |
| **Khả dụng (Availability)**                  | NFR5   | Thời gian hoạt động    | Hệ thống hoạt động liên tục 99.5% thời gian trong tháng.                             |
| **Khả năng mở rộng (Scalability)**           | NFR6   | Mở rộng hạ tầng        | Cho phép mở rộng máy chủ khi lượng người học tăng cao.                               |
| **Tính tương thích (Compatibility)**         | NFR7   | Hỗ trợ đa nền tảng     | Hệ thống chạy được trên trình duyệt web, điện thoại (Android, iOS).                  |
| **Khả năng bảo trì (Maintainability)**       | NFR8   | Dễ bảo trì             | Mã nguồn có cấu trúc rõ ràng, tài liệu đầy đủ, tuân thủ mô hình MVC.                 |
| **Giao diện người dùng (Usability)**         | NFR9   | Thân thiện, dễ sử dụng | Giao diện trực quan, hỗ trợ người dùng không chuyên về CNTT.                         |
| **Sao lưu và khôi phục (Backup & Recovery)** | NFR10  | Sao lưu dữ liệu        | Hệ thống sao lưu dữ liệu tự động mỗi ngày, có cơ chế khôi phục nhanh khi xảy ra lỗi. |

