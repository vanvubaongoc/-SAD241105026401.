
 Tài liệu thiết kế hệ thống "Payroll System"

---

## 1. Mô tả chung
Hệ thống "Payroll System" được thiết kế để quản lý quá trình xử lý lương và hỗ trợ các hoạt động liên quan như thanh toán ngân hàng, in phiếu lương, và quản lý thông tin về dự án. Dựa trên các phân tích ca sử dụng và các phần tử thiết kế, tài liệu này trình bày chi tiết các ca sử dụng, mô hình thiết kế, và lý do lựa chọn các thành phần.

---

## 2. Danh sách các ca sử dụng chính
Dựa trên phân tích hệ thống, các ca sử dụng chính bao gồm:

1. **Xử lý thanh toán trực tiếp qua ngân hàng**
   - **Miêu tả**: Xử lý việc thanh toán trực tiếp lương vào tài khoản ngân hàng của nhân viên.
   - **Thành phần chính**:
     - `PayrollController`: Điều phối quy trình xử lý lương.
     - `IBankSystem`: Giao tiếp với hệ thống ngân hàng để thực hiện thanh toán.
     - `BankSystem`: Subsystem thực hiện chi tiết việc thanh toán.

2. **In phiếu lương**
   - **Miêu tả**: In phiếu lương dưới dạng văn bản trên máy in được chỉ định.
   - **Thành phần chính**:
     - `PayrollController`: Điều phối việc xử lý in phiếu lương.
     - `IPrintService`: Giao tiếp với máy in.
     - `PrintService`: Subsystem quản lý việc in phiếu.
