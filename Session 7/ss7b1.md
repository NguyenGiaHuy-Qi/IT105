1. Kiến trúc tổng thể

- Hệ thống được thiết kế theo mô hình Client–Server với kiến trúc Microservices hoặc Modular Monolith tùy quy mô

#### Các lớp chính:

| Lớp                   | Vai trò                                                                          |
| --------------------- | -------------------------------------------------------------------------------- |
| **Frontend**          | Giao diện người dùng trên web và mobile (hiển thị dữ liệu, tương tác người dùng) |
| **Backend (API)**     | Cung cấp các dịch vụ và xử lý logic nghiệp vụ thông qua RESTful API hoặc GraphQL |
| **Database**          | Lưu trữ dữ liệu sản phẩm, người dùng, đơn hàng, thanh toán                       |
| **External Services** | Tích hợp các dịch vụ bên ngoài: thanh toán, vận chuyển, email, SMS, v.v.         |


2. Cấu trúc chi tiết hệ thống

    1. Frontend

    - Viết bằng React
    - Giao tiếp với Backend qua API (HTTPS/JSON)
    - Quản lý session (JWT)


    **Chức năng:**
    - Đăng nhập/đăng ký
    - Tìm kiếm và xem chi tiết sản phẩm
    - Quản lý giỏ hàng
    - Thanh toán và xem trạng thái đơn hàng
    - Quản lý tài khoản cá nhân


    2. Backend (API Server)

    - Viết bằng Node.js, Java Spring Boot, hoặc .NET Core
    - Cung cấp các module chính:
    - User Service: quản lý tài khoản, xác thực (JWT/OAuth2)
    - Product Service: quản lý danh mục, sản phẩm, tồn kho
    - Order Service: quản lý đơn hàng, giỏ hàng, hóa đơn
    - Payment Service: kết nối với cổng thanh toán (VNPay, Momo, PayPal, v.v.)
    - Notification Service: gửi email, SMS, hoặc push notification
    - Shipping Service: tích hợp với đơn vị vận chuyển (Giao hàng nhanh, Viettel Post, v.v.)


    3. Database Layer
    **CSDL chính:**
    - PostgreSQL / MySQL (dữ liệu giao dịch, người dùng, sản phẩm)
    - Redis (cache phiên đăng nhập, giỏ hàng tạm thời)
    - MongoDB (nếu cần lưu trữ dữ liệu phi cấu trúc: log, đánh giá sản phẩm)

    **Các bảng chính:**
    users, products, categories, orders, order_items, payments, shipments, carts

    
    4. External Services

    - Cổng thanh toán: VNPay, Momo, PayPal
    - Vận chuyển: Giao hàng nhanh, Viettel Post API
    - Email/SMS: SendGrid, Twilio, Zalo ZNS
    - Analytics: Google Analytics / Firebase Analytics


3. Sơ đồ kiến trúc tổng thể:

![Ex1](/Session07/assets/Ex1-SS7.jpg)