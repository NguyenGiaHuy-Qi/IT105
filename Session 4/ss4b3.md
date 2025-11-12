

| Thành phần        | Modifier (Phạm vi truy cập) | Giải thích |
|------------------|----------------------------|------------|
| `username`        | `private`                 | Thông tin nhạy cảm, không muốn truy cập trực tiếp từ bên ngoài. Có thể cung cấp getter/setter nếu cần. |
| `password`        | `private`                 | Rất nhạy cảm, cần bảo vệ tuyệt đối, không cho phép truy cập trực tiếp từ bên ngoài. |
| `login()`         | `public`                  | Phương thức cần gọi từ bên ngoài (ví dụ UI, controller) để đăng nhập. |
| `resetPassword()` | `public`                  | Cho phép người dùng hoặc hệ thống gọi từ bên ngoài để đặt lại mật khẩu. |
| `lastLoginTime`   | `private`                 | Không muốn cho truy cập trực tiếp; có thể cung cấp getter nếu cần tra cứu lần đăng nhập gần nhất. |
