# 3. Xác định các phần tử thiết kế

Phần này xác định các phần tử thiết kế chính của hệ thống Mentcare, mô tả cách chúng được tổ chức và các cơ chế thiết kế được sử dụng để đáp ứng các yêu cầu đã nêu.

---

## 3.1 Các phần tử thiết kế chính

Hệ thống Mentcare được thiết kế dựa trên kiến trúc **client-server** với các phần tử chính sau:

### 1. Cơ sở dữ liệu (Database)
- Sử dụng cơ sở dữ liệu quan hệ để lưu trữ thông tin.
- **Các bảng chính**:
  - **Hồ sơ bệnh nhân (Patient Records):** Lưu trữ thông tin cá nhân, lịch sử khám, đánh giá rủi ro và thông tin chẩn đoán.
  - **Lịch sử tư vấn (Consultation History):** Ghi nhận thông tin chi tiết về các buổi tư vấn.
  - **Thông tin thuốc (Medication Information):** Ghi nhận các đơn thuốc, lịch sử kê đơn và thông tin tác dụng phụ.
  - **Dữ liệu pháp lý (Legal Compliance Records):** Theo dõi các quy trình tuân thủ Luật Sức khỏe Tâm thần.

### 2. Ứng dụng phía máy khách (Client Application)
- Giao diện dựa trên trình duyệt Firefox.
- **Chức năng chính**:
  - Quản lý thông tin bệnh nhân.
  - Theo dõi triệu chứng và lịch sử điều trị.
  - Quản lý lịch hẹn và báo cáo.

### 3. Ứng dụng phía máy chủ (Server Application)
- Chịu trách nhiệm xử lý logic nghiệp vụ.
- **Hỗ trợ các chức năng**:
  - Xác thực người dùng.
  - Quản lý kết nối với cơ sở dữ liệu.
  - Theo dõi rủi ro bệnh nhân và xử lý các cảnh báo.

### 4. Tích hợp hệ thống bên ngoài
- Tích hợp với:
  - **Hệ thống quốc gia về hồ sơ bệnh nhân (National Patient Record System).**
  - **Hệ thống quản lý thuốc (Drug Information System).**
  - **Hệ thống lịch hẹn (APPOINTMENTS).**

### 5. Cơ chế bảo mật
- Hỗ trợ kiểm soát truy cập dựa trên vai trò (RBAC).
- Mã hóa toàn bộ dữ liệu đầu cuối và lưu trữ log truy cập.

---

## 3.2 Cơ chế thiết kế

### 1. Quản lý người dùng và phân quyền
- Xác thực đa yếu tố với mật khẩu và câu hỏi bảo mật.
- Quản lý quyền truy cập theo vai trò: bác sĩ, quản trị viên, nhân viên hỗ trợ.

### 2. Quản lý dữ liệu an toàn
- Mã hóa thông tin bệnh nhân để đảm bảo tính bảo mật.
- Kiểm tra và phát hiện dữ liệu sai lệch hoặc thiếu sót.

### 3. Tự động hóa quy trình
- Hỗ trợ cảnh báo khi phát hiện nguy cơ rủi ro (tự tử, tác dụng phụ của thuốc).
- Tự động đồng bộ hóa dữ liệu khi sử dụng trên máy tính xách tay ngoại tuyến.

### 4. Tối ưu hóa hiệu năng
- Đảm bảo thời gian phản hồi dưới 2 giây cho các thao tác thông thường.
- Chạy trên máy chủ Linux với giới hạn bộ nhớ tối đa 32GB.

### 5. Tạo báo cáo và in ấn
- Báo cáo cá nhân hóa dành cho bác sĩ và báo cáo ẩn danh cho quản lý.
- Tùy chọn in hồ sơ hoặc các thành phần báo cáo cụ thể.

### 6. Kiểm tra và đảm bảo tuân thủ pháp lý
- Theo dõi nhật ký hoạt động để phục vụ kiểm tra pháp lý.
- Đảm bảo tuân thủ Luật Bảo vệ Dữ liệu và Luật Sức khỏe Tâm thần.

---

## 3.3 Tổ chức phần tử thiết kế

Các phần tử thiết kế sẽ được tổ chức thành các module chính như sau:

- **Module quản lý bệnh nhân:** 
  - Tạo, cập nhật, lưu trữ thông tin bệnh nhân.
  - Theo dõi rủi ro và lịch sử chẩn đoán.
  
- **Module quản lý lịch hẹn:** 
  - Tích hợp với hệ thống APPOINTMENTS để quản lý lịch hẹn.

- **Module phân tích rủi ro:** 
  - Phát hiện nguy cơ tự tử, bạo lực và tương tác thuốc nguy hiểm.

- **Module báo cáo:** 
  - Tạo và quản lý báo cáo cá nhân hóa hoặc ẩn danh.

- **Module bảo mật:** 
  - Xác thực, mã hóa, và phân quyền.

---

Hệ thống Mentcare được thiết kế tập trung vào độ tin cậy, tính bảo mật và khả năng sử dụng, đáp ứng các yêu cầu đặc thù của lĩnh vực sức khỏe tâm thần và các quy định pháp lý.
