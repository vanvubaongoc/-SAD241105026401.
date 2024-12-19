# BÁO CÁO CUỐI KÌ 
## Mentcare: A mental health support system

#  I.Tóm Tắt Bài Toán Mentcare

Bài toán yêu cầu thiết kế một hệ thống thông tin sức khỏe tâm thần với yêu cầu cao về độ tin cậy, bảo mật và tuân thủ pháp luật, đồng thời giải quyết xung đột giữa bảo mật thông tin và an toàn bệnh nhân. Đây là một trường hợp điển hình để nghiên cứu các khía cạnh về kỹ thuật yêu cầu, quản lý xung đột và phát triển hệ thống phụ thuộc cao.

## Sự Cần Thiết Khi Giải Quyết Bài Toán Mentcare

1. **Đảm bảo an toàn cho bệnh nhân và nhân viên y tế**:
    - Với tính chất là một hệ thống an toàn thứ cấp, sự thất bại của Mentcare có thể dẫn đến hậu quả nghiêm trọng như sai sót trong điều trị, gây nguy hiểm cho cả bệnh nhân và nhân viên y tế. Hệ thống đáng tin cậy là nền tảng để đưa ra các quyết định y tế đúng đắn.

2. **Quản lý thông tin chuyên biệt cho sức khỏe tâm thần**:
    - Sức khỏe tâm thần đòi hỏi quản lý thông tin chi tiết hơn so với các lĩnh vực y tế khác. Việc thiết kế hệ thống chuyên biệt giúp theo dõi sát sao tình trạng bệnh nhân, từ đó hỗ trợ quá trình điều trị hiệu quả hơn.

3. **Tuân thủ các quy định pháp luật**:
    - Sức khỏe tâm thần là một lĩnh vực nhạy cảm với các yêu cầu pháp lý đặc thù. Một hệ thống như Mentcare cần đảm bảo sự tuân thủ luật pháp về bảo mật, quyền riêng tư và quản lý hồ sơ.

4. **Hỗ trợ ra quyết định y tế**:
    - Hệ thống cung cấp thông tin chi tiết và chính xác, hỗ trợ các bác sĩ và nhân viên y tế đưa ra quyết định điều trị hiệu quả, giảm thiểu sai sót và tối ưu hóa quy trình chăm sóc.

## Lợi Ích Khi Giải Quyết Bài Toán Mentcare

1. **Cải thiện chất lượng chăm sóc sức khỏe tâm thần**:
    - Việc theo dõi và lưu trữ thông tin một cách chi tiết giúp bác sĩ có cái nhìn toàn diện hơn về bệnh nhân, từ đó cải thiện hiệu quả điều trị.

2. **Bảo mật và quản lý dữ liệu tốt hơn**:
    - Hệ thống giảm nguy cơ lộ lọt thông tin nhạy cảm của bệnh nhân, đảm bảo quyền riêng tư trong khi vẫn duy trì khả năng truy cập thông tin cần thiết khi cần thiết.

3. **Tăng cường sự an toàn**:
    - Bằng cách cung cấp dữ liệu kịp thời và đáng tin cậy, hệ thống giúp giảm nguy cơ đưa ra các quyết định không chính xác, bảo vệ sự an toàn của bệnh nhân và nhân viên y tế.

4. **Tiết kiệm thời gian và nguồn lực**:
    - Tự động hóa quy trình tạo báo cáo, thư từ và quản lý hồ sơ giúp giảm thiểu công việc thủ công, từ đó tiết kiệm thời gian và nguồn lực.

5. **Giải quyết xung đột giữa bảo mật và an toàn**:
    - Việc giải quyết xung đột giữa các yêu cầu đảm bảo quyền riêng tư và an toàn sẽ tạo ra một hệ thống cân bằng, đáp ứng được cả hai tiêu chí quan trọng này.

6. **Tạo tiền đề cho các nghiên cứu và cải tiến**:
    - Hệ thống Mentcare cung cấp một nền tảng dữ liệu phong phú, hỗ trợ các nghiên cứu khoa học về sức khỏe tâm thần và phát triển các phương pháp điều trị mới.

7. **Ứng dụng trong đào tạo và phát triển chuyên môn**:
    - Hệ thống là công cụ hữu ích để đào tạo nhân viên y tế về các quy trình tuân thủ pháp luật và thực hành y tế tốt nhất.

## Các Yêu Cầu Chức Năng (Functional Requirements)

1. **Quản lý thông tin bệnh nhân**:
    - Tạo, cập nhật, lưu trữ và quản lý hồ sơ bệnh nhân bao gồm thông tin cá nhân, đánh giá rủi ro, chẩn đoán, điều trị và đơn thuốc.
    - Cung cấp khả năng nhập nhận xét tự do của bác sĩ để xử lý các trường hợp phức tạp.
    - Theo dõi lịch sử khám bệnh và đơn thuốc của bệnh nhân.

2. **Hỗ trợ chẩn đoán và điều trị**:
    - Hiển thị các tác dụng phụ của thuốc và cảnh báo trong trường hợp dị ứng thuốc.
    - Theo dõi tình trạng rủi ro tự tử hoặc nguy hiểm của bệnh nhân.
    - Quản lý bệnh nhân bị giữ (sectioned) và đảm bảo thực hiện các quy trình pháp lý.

3. **Hỗ trợ báo cáo**:
    - Tạo báo cáo cá nhân hóa cho nhân viên y tế và báo cáo ẩn danh cho quản lý.
    - Cung cấp khả năng in hồ sơ hoặc báo cáo theo yêu cầu.

4. **Hỗ trợ quản lý cuộc hẹn**:
    - Tích hợp với hệ thống đặt lịch hẹn (APPOINTMENTS) để quản lý thông tin cuộc hẹn.
    - Theo dõi và ghi nhận tình trạng bệnh nhân vắng mặt trong cuộc hẹn.

5. **Hỗ trợ nhân viên y tế di động**:
    - Cho phép tải xuống, cập nhật và đồng bộ hóa hồ sơ bệnh nhân trên máy tính xách tay khi thăm khám tại nhà.

## Các Yêu Cầu Phi Chức Năng (Non-functional Requirements)

1. **Yêu cầu về hiệu suất**:
    - Hệ thống phải phản hồi trong vòng 2 giây đối với các truy vấn thông thường.
    - Đảm bảo tính khả dụng từ 8h00 đến 18h30 từ thứ Hai đến thứ Sáu.

2. **Yêu cầu về bảo mật**:
    - Sử dụng hệ thống kiểm soát truy cập dựa trên vai trò (Role-based Access Control).
    - Mã hóa tất cả dữ liệu và đảm bảo chỉ nhân viên được ủy quyền mới có quyền truy cập thông tin.
    - Không cho phép sao lưu hoặc sao chép dữ liệu lên thiết bị lưu trữ di động.

3. **Yêu cầu về quyền riêng tư**:
    - Tuân thủ các điều khoản của Đạo luật Bảo vệ Dữ liệu (Data Protection Act) năm 1998.
    - Đảm bảo dữ liệu bệnh nhân được ẩn danh trong các báo cáo nghiên cứu.

4. **Yêu cầu về khả năng tương tác**:
    - Tích hợp với hệ thống quốc gia về hồ sơ bệnh nhân (National Patient Record System) và hệ thống quản lý thuốc.
    - Sử dụng phần mềm mã nguồn mở và trình duyệt Firefox làm tiêu chuẩn.

5. **Yêu cầu về an toàn**:
    - Cảnh báo bác sĩ về những rủi ro như tự tử, bạo lực, hoặc tác dụng phụ của thuốc.
    - Theo dõi việc kê đơn và phát hiện các đơn thuốc tiềm ẩn vấn đề.

6. **Yêu cầu về sử dụng**:
    - Giao diện dựa trên biểu mẫu dễ sử dụng, hỗ trợ nhân viên nhanh chóng làm quen.
    - Giảm thiểu sai sót của người dùng thông qua kiểm tra đầu vào và sử dụng các menu lựa chọn sẵn.

7. **Yêu cầu về hệ thống**:
    - Chạy trên máy chủ Linux với giới hạn bộ nhớ 32GB.
    - Hỗ trợ sao lưu và khôi phục dữ liệu khi có sự cố.
# II.Phân tích các ca sử dụng

## Kiến trúc và mô hình triển khai:
- **Máy khách và máy chủ**:
  + **Máy khách**: Nhân viên y tế và quản trị viên sẽ truy cập hệ thống qua trình duyệt web (Firefox) với giao diện người dùng dưới dạng biểu mẫu, giúp thực hiện các tác vụ nhập liệu và chỉnh sửa hồ sơ.
  + **Máy chủ**: Đảm nhận việc lưu trữ hồ sơ bệnh nhân và xử lý các yêu cầu từ máy khách. Hệ thống được triển khai trên các máy chủ Linux để đảm bảo tính ổn định và bảo mật.

---

## Các yêu cầu hệ thống:

- **Khả năng vận hành**:
  + Hệ thống phải duy trì hoạt động ổn định từ 08:30 sáng đến 17:00 chiều từ Thứ Hai đến Thứ Sáu.
  + Các công tác bảo trì hệ thống sẽ được thực hiện ngoài giờ hành chính (từ 22:00 đến 00:30, hoặc vào sáng Chủ Nhật từ 07:30 đến 11:30).

- **Hiệu suất**:
  + Hệ thống cần có thời gian phản hồi dưới 2 giây cho các truy vấn bệnh nhân thông thường.
  + Nếu hệ thống mất thời gian phản hồi trên 2 giây, sẽ có thông báo cho người sử dụng về tình trạng xử lý hiện tại.

- **Bảo mật**:
  + Hệ thống phải đảm bảo bảo mật tuyệt đối thông tin bệnh nhân, chỉ những nhân viên có quyền mới có thể truy cập dữ liệu.
  + Hệ thống cần tích hợp cơ chế xác thực hai yếu tố để tăng cường độ an toàn.

- **Quản lý dữ liệu**:
  + Trước khi lưu trữ, dữ liệu cần được kiểm tra tính hợp lệ, đặc biệt là các trường không có sẵn trong danh sách lựa chọn.
  + Mọi thông tin cần tuân thủ các quy định về bảo mật và chuẩn mực của hệ thống y tế Mid-Scotland.

---

## Kết quả phân tích từng trường hợp sử dụng:

### 1. **Quản lý chăm sóc cá nhân**:
- **Mô tả ngắn**: Ca sử dụng này cho phép nhân viên lâm sàng thực hiện các thao tác quản lý thông tin bệnh nhân như tạo hồ sơ, sửa đổi dữ liệu và xem lịch sử điều trị.
  
- **Quy trình**:
  - **Quy trình cơ bản**:
    + Nhân viên lâm sàng đăng nhập vào hệ thống.
    + Hệ thống hiển thị giao diện tìm kiếm hồ sơ bệnh nhân.
    + Nhân viên tìm kiếm hoặc chọn bệnh nhân từ danh sách.
    + Nhân viên xem hoặc cập nhật thông tin bệnh nhân, hoặc tạo hồ sơ mới.
    + Hệ thống xác nhận và lưu thay đổi vào cơ sở dữ liệu.
  - **Trường hợp thay thế**:
    + **AF1**: Nếu không tìm thấy bệnh nhân, hệ thống sẽ thông báo và cho phép tạo hồ sơ mới.
    + **AF2**: Nếu dữ liệu nhập không hợp lệ, hệ thống sẽ hiển thị lỗi và yêu cầu chỉnh sửa.

- **Yêu cầu đặc biệt**:
  + Cần xác thực thông tin đăng nhập của nhân viên.
  + Kiểm tra tính hợp lệ của dữ liệu nhập vào, bao gồm định dạng và tính chính xác.

- **Điều kiện tiên quyết**:
  + Nhân viên đã đăng nhập thành công vào hệ thống.
  + Cơ sở dữ liệu bệnh nhân phải sẵn sàng.

- **Điều kiện hậu**:
  + Hồ sơ bệnh nhân được tạo hoặc cập nhật thành công.
  + Thay đổi được lưu trữ trong cơ sở dữ liệu một cách an toàn.

- **Điểm mở rộng**: Tích hợp với hệ thống hồ sơ quốc gia: Khi tạo hoặc chỉnh sửa hồ sơ, thông tin có thể được gửi tới hệ thống hồ sơ bệnh án quốc gia.

### 2. **Theo dõi tình trạng bệnh nhân**:
- **Mô tả ngắn**: Hệ thống theo dõi tình trạng bệnh nhân, cảnh báo các vấn đề như bỏ lỡ cuộc hẹn hoặc nguy cơ sức khỏe và thông báo cho nhân viên lâm sàng.

- **Quy trình**:
  - **Quy trình cơ bản**:
    + Hệ thống kiểm tra tự động hồ sơ bệnh nhân định kỳ.
    + Nếu phát hiện vấn đề (bỏ lỡ cuộc hẹn hoặc không tuân thủ điều trị), hệ thống gửi cảnh báo.
    + Nhân viên nhận thông báo qua giao diện hoặc email.
  - **Trường hợp thay thế**:
    + **AF1**: Nếu không phát hiện vấn đề, hệ thống không gửi cảnh báo.
    + **AF2**: Nếu thông tin lịch sử không đầy đủ, hệ thống sẽ thông báo lỗi cho quản trị viên.

- **Yêu cầu đặc biệt**:
  + Hệ thống phải thực hiện kiểm tra tự động mỗi ngày.
  + Dữ liệu lịch sử bệnh nhân phải chính xác để đưa ra cảnh báo hợp lý.

- **Điều kiện tiên quyết**:
  + Hồ sơ bệnh nhân có đủ dữ liệu.
  + Nhân viên đã được cấp quyền nhận thông báo.

- **Điều kiện hậu**:
  + Cảnh báo sẽ được gửi tới nhân viên lâm sàng.
  + Các hành động cần thiết (nếu có) sẽ được thực hiện.

- **Điểm mở rộng**: Tích hợp với hệ thống quản lý lịch hẹn: Dữ liệu lịch hẹn sẽ được so sánh với hồ sơ bệnh nhân để xác minh sự tuân thủ điều trị.

### 3. **Quản lý giam giữ bắt buộc**:
- **Mô tả ngắn**: Cập nhật và quản lý thông tin bệnh nhân bị giam giữ tại bệnh viện để tuân thủ các quy định pháp lý.

- **Quy trình**:
  - **Quy trình cơ bản**:
    + Nhân viên lâm sàng cập nhật thông tin giam giữ của bệnh nhân.
    + Hệ thống xác nhận thông tin nhập vào (ngày giam giữ, lý do).
    + Dữ liệu được lưu trữ trong hệ thống.
    + Hệ thống sẽ gửi thông báo nhắc nhở về các cuộc kiểm tra định kỳ.
  - **Trường hợp thay thế**:
    + **AF1**: Nếu dữ liệu không hợp lệ, hệ thống sẽ yêu cầu sửa chữa và gửi lại.

- **Yêu cầu đặc biệt**:
  + Phải tuân thủ các quy định pháp lý về giam giữ bắt buộc.
  + Đảm bảo bảo mật cao cho thông tin dữ liệu.

- **Điều kiện tiên quyết**:
  + Nhân viên lâm sàng có quyền chỉnh sửa thông tin giam giữ.
  + Hệ thống phải hoạt động ổn định và có thể truy cập.

- **Điều kiện hậu**:
  + Thông tin giam giữ được cập nhật chính xác.
  + Lịch kiểm tra liên quan được lên kế hoạch và nhắc nhở.

- **Điểm mở rộng**: Tích hợp với hệ thống báo cáo quản lý: Thông tin giam giữ sẽ được đưa vào các báo cáo hành chính.

### 4. **Báo cáo hành chính**:
- **Mô tả ngắn**: Tạo các báo cáo ẩn danh về số lượng bệnh nhân, chi phí điều trị, và các chỉ số quản lý.

- **Quy trình**:
  - **Quy trình cơ bản**:
    + Quản trị viên chọn loại báo cáo cần tạo.
    + Hệ thống thu thập dữ liệu và tạo báo cáo.
    + Báo cáo được lưu trữ và sẵn sàng để tải xuống hoặc in.
  - **Trường hợp thay thế**:
    + **AF1**: Nếu không có đủ dữ liệu, hệ thống sẽ yêu cầu kiểm tra lại.

- **Yêu cầu đặc biệt**:
  + Báo cáo cần được ẩn danh để bảo vệ quyền riêng tư của bệnh nhân.
  + Thời gian tạo báo cáo không quá 10 giây.

- **Điều kiện tiên quyết**:
  + Dữ liệu cần thiết đã được ghi nhận đầy đủ trong hệ thống.
  + Quản trị viên có quyền tạo báo cáo.

- **Điều kiện hậu**:
  + Báo cáo được lưu trữ và có sẵn cho sử dụng.
  + Hệ thống ghi lại lịch sử tạo báo cáo.

- **Điểm mở rộng**: Tích hợp với hệ thống quản lý cấp cao: Các báo cáo có thể được chia sẻ trực tiếp với các nhà quản lý cấp cao qua email.
