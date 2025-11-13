1. Xác định loại Hệ thống thông tin phù hợp


| **Mức độ hệ thống**                        | **Tên hệ thống**                  | **Chức năng trong doanh nghiệp logistics**                                 | **Giải thích vì sao phù hợp**                                          |
| ------------------------------------------ | --------------------------------- | -------------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| **1. TPS (Transaction Processing System)** | **Hệ thống xử lý giao dịch**      | Quản lý nhập đơn hàng, cập nhật trạng thái, ghi nhận thời gian giao hàng   | Xử lý dữ liệu giao dịch hằng ngày, đảm bảo tính chính xác và tốc độ.   |
| **2. MIS (Management Information System)** | **Hệ thống thông tin quản lý**    | Tổng hợp dữ liệu đơn hàng, tạo báo cáo doanh thu, hiệu suất giao hàng      | Cung cấp báo cáo cho quản lý trung cấp, hỗ trợ ra quyết định vận hành. |
| **3. DSS (Decision Support System)**       | **Hệ thống hỗ trợ ra quyết định** | Phân tích tuyến đường, tối ưu vận tải, dự đoán thời gian giao hàng         | Hỗ trợ ra quyết định dựa trên dữ liệu và mô hình phân tích.            |
| **4. EIS (Executive Information System)**  | **Hệ thống thông tin điều hành**  | Cung cấp báo cáo tổng hợp cho lãnh đạo (KPI, chi phí, thời gian giao hàng) | Phục vụ chiến lược dài hạn, quản lý toàn doanh nghiệp.                 |


### Kết luận loại hệ thống phù hợp:

Hệ thống kết hợp TPS + MIS + DSS là phù hợp nhất:

TPS: để quản lý và theo dõi đơn hàng hàng ngày.

MIS: để tổng hợp và báo cáo hiệu quả giao hàng.

DSS: để hỗ trợ tối ưu tuyến đường và lập kế hoạch vận chuyển.

Nếu doanh nghiệp muốn quản lý cấp cao hơn (phân tích tổng thể, KPI, chi phí), có thể mở rộng thêm EIS trong giai đoạn phát triển sau.


2. Lựa chọn mô hình phát triển phần mềm


| **Mô hình**                | **Đặc điểm chính**                                                                             | **Ưu điểm**                                                           | **Nhược điểm**                                           | **Mức độ phù hợp**                                                               |
| -------------------------- | ---------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------------------------- |
| **Waterfall (Thác nước)**  | Phát triển tuần tự qua các giai đoạn: phân tích → thiết kế → lập trình → kiểm thử → triển khai | Phù hợp với yêu cầu ổn định, dễ kiểm soát tiến độ                     | Khó thay đổi khi yêu cầu phát sinh                       |   Không linh hoạt cho hệ thống logistics (yêu cầu thường thay đổi)               |
| **Agile (Linh hoạt)**      | Phát triển theo vòng lặp (sprint), phản hồi liên tục, cải tiến liên tục                        | Thích hợp với dự án có yêu cầu thay đổi, người dùng tham gia liên tục | Cần phối hợp chặt chẽ giữa nhóm phát triển và khách hàng |   Rất phù hợp vì hệ thống logistics thường cần điều chỉnh theo thực tế giao hàng |
| **Scrum (một dạng Agile)** | Phân chia công việc theo sprint ngắn, họp đánh giá định kỳ                                     | Linh hoạt, kiểm thử sớm, dễ thích ứng                                 | Phụ thuộc vào sự hợp tác của đội nhóm                    |   Rất phù hợp                                                                    |
| **Prototyping (Mẫu thử)**  | Xây dựng mô hình thử nghiệm, lấy phản hồi người dùng, rồi phát triển hoàn thiện                | Giúp hiểu rõ yêu cầu trước khi phát triển chính thức                  | Tốn thời gian giai đoạn đầu                              | ✔ Phù hợp nếu khách hàng chưa rõ yêu cầu ban đầu                                 |
| **DevOps**                 | Tích hợp phát triển và vận hành liên tục (CI/CD)                                               | Triển khai nhanh, phản hồi tức thời, giám sát hiệu quả                | Cần hạ tầng kỹ thuật cao                                 | ✔ Phù hợp nếu công ty có quy mô lớn, yêu cầu vận hành 24/7                       |


### Kết luận mô hình phát triển phù hợp:

Agile (hoặc Scrum) là mô hình phát triển thích hợp nhất cho hệ thống quản lý giao hàng online, vì:

Yêu cầu thực tế trong logistics thay đổi thường xuyên (điều phối, tuyến đường, khách hàng mới).

Cần phản hồi nhanh từ người dùng (nhân viên giao hàng, điều phối viên).

Hệ thống cần triển khai theo từng giai đoạn, có thể nâng cấp dần (module theo dõi, tối ưu, phân tích).