# Thiết Kế Hệ Thống Con cho Payroll System

## 1. Phân hệ Giao diện Người Dùng (UI Subsystem)

### 1.1. Phân bổ hành vi
- **Nhận và hiển thị thông tin đăng nhập từ người dùng**: Giao diện người dùng cung cấp các trường nhập liệu để người dùng nhập thông tin như email và mật khẩu.
- **Hiển thị thông báo lỗi nếu thông tin đăng nhập không hợp lệ**: Khi thông tin nhập vào không hợp lệ, thông báo lỗi sẽ được hiển thị để người dùng điều chỉnh.

### 1.2. Tài liệu các phần tử
- **LoginPage**: Giao diện người dùng để nhập thông tin đăng nhập.
- **LoginController**: Quản lý các sự kiện và tương tác của người dùng với giao diện.

### 1.3. Sự phụ thuộc
- Phụ thuộc vào **Authentication Subsystem** để xử lý thông tin đăng nhập và trả về kết quả.

### 1.4. UML
Đề xuất UML cho phân hệ Giao diện Người Dùng:
