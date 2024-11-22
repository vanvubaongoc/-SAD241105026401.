# Lab 2

## 1. Phân tích ca sử dụng:

### Maintain Timecard
- **Mô tả:** Nhân viên hoặc quản lý nhập thông tin chấm công (timecard) vào hệ thống.
- **Actor:** Nhân viên, Quản lý
- **Các bước thực hiện:**
  1. Nhân viên đăng nhập vào hệ thống.
  2. Chọn tùy chọn "Maintain Timecard".
  3. Nhập thông tin chấm công bao gồm: ngày làm việc, số giờ làm việc, và mã nhân viên.
  4. Lưu thông tin chấm công vào cơ sở dữ liệu.
  5. Hệ thống hiển thị thông báo cập nhật thành công.
- **Ngoại lệ:**
  - Thông tin nhập không hợp lệ (ví dụ: số giờ làm vượt quá giới hạn).
  - Nhân viên không có quyền truy cập vào chức năng này.

### Calculate Payroll
- **Mô tả:** Hệ thống tính toán bảng lương cho nhân viên dựa trên thông tin chấm công và bảng lương cơ bản.
- **Actor:** Hệ thống, Quản lý
- **Các bước thực hiện:**
  1. Hệ thống truy xuất thông tin chấm công của nhân viên.
  2. Tính toán tổng thu nhập dựa trên giờ làm việc và lương cơ bản.
  3. Trừ các khoản khấu trừ (bảo hiểm, thuế).
  4. Cập nhật thông tin vào bảng lương và hiển thị cho quản lý.

### Select Payment Method
- **Mô tả:** Nhân viên chọn phương thức thanh toán lương (chuyển khoản ngân hàng, tiền mặt).
- **Actor:** Nhân viên
- **Các bước thực hiện:**
  1. Nhân viên đăng nhập vào hệ thống.
  2. Chọn tùy chọn "Select Payment Method".
  3. Chọn phương thức thanh toán mong muốn.
  4. Hệ thống lưu lại thông tin lựa chọn.

### View Pay Statement
- **Mô tả:** Nhân viên có thể xem bảng lương của mình.
- **Actor:** Nhân viên
- **Các bước thực hiện:**
  1. Nhân viên đăng nhập vào hệ thống.
  2. Chọn tùy chọn "View Pay Statement".
  3. Hệ thống hiển thị bảng lương cho nhân viên.

## 3. Java mô phỏng ca sử dụng: Maintain Timecard

Dưới đây là mã nguồn Java mô phỏng chức năng **Maintain Timecard**:

```java
import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;

class Timecard {
    private String employeeId;
    private String workDate;
    private int hoursWorked;

    public Timecard(String employeeId, String workDate, int hoursWorked) {
        this.employeeId = employeeId;
        this.workDate = workDate;
        this.hoursWorked = hoursWorked;
    }

    public String getEmployeeId() {
        return employeeId;
    }

    public String getWorkDate() {
        return workDate;
    }

    public int getHoursWorked() {
        return hoursWorked;
    }

    @Override
    public String toString() {
        return "Employee ID: " + employeeId + ", Work Date: " + workDate + ", Hours Worked: " + hoursWorked;
    }
}

class TimecardService {
    private List<Timecard> timecards = new ArrayList<>();

    public void addTimecard(Timecard timecard) {
        timecards.add(timecard);
        System.out.println("Timecard added successfully.");
    }

    public void displayTimecards() {
        if (timecards.isEmpty()) {
            System.out.println("No timecards found.");
            return;
        }

        System.out.println("Timecards List:");
        for (Timecard timecard : timecards) {
            System.out.println(timecard);
        }
    }
}

public class MaintainTimecardApp {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        TimecardService timecardService = new TimecardService();

        while (true) {
            System.out.println("\n=== Maintain Timecard ===");
            System.out.println("1. Add Timecard");
            System.out.println("2. View Timecards");
            System.out.println("3. Exit");
            System.out.print("Choose an option: ");
            int choice = scanner.nextInt();

            switch (choice) {
                case 1:
                    System.out.print("Enter Employee ID: ");
                    String employeeId = scanner.next();
                    System.out.print("Enter Work Date (YYYY-MM-DD): ");
                    String workDate = scanner.next();
                    System.out.print("Enter Hours Worked: ");
                    int hoursWorked = scanner.nextInt();

                    if (hoursWorked < 0 || hoursWorked > 24) {
                        System.out.println("Invalid hours worked. Please enter a value between 0 and 24.");
                    } else {
                        Timecard timecard = new Timecard(employeeId, workDate, hoursWorked);
                        timecardService.addTimecard(timecard);
                    }
                    break;
                case 2:
                    timecardService.displayTimecards();
                    break;
                case 3:
                    System.out.println("Exiting the application.");
                    scanner.close();
                    return;
                default:
                    System.out.println("Invalid choice. Please try again.");
            }
        }
    }
}
```
