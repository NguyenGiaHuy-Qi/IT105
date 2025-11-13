## Phân rã hệ thống thành các module:

1. Presentation Layer
- Modules:
    + PostController → quản lý hiển thị bài viết (danh sách, chi tiết, tạo, chỉnh sửa).
    + CommentController → hiển thị và gửi bình luận.
    + UserController → đăng ký, đăng nhập, quản lý hồ sơ.

2. Business Logic Layer
- Modules:
    + PostService
        Xử lý tạo, cập nhật, xóa, tìm kiếm bài viết.

        Kiểm tra quyền của người viết.

    + CommentService
        Quản lý bình luận, kiểm tra nội dung hợp lệ, lọc spam.

    + UserService
        Quản lý người dùng, xác thực (login), phân quyền (admin, user).

3. Data Access Layer
- Modules:
    + PostRepository → thao tác CRUD với bảng posts.
    + CommentRepository → thao tác CRUD với bảng comments.
    + UserRepository → lưu và truy vấn thông tin người dùng.


## Sơ đồ lớp (Class Diagram) 

![Ex5](/Session07/assets/Ex5-SS7.jpg)