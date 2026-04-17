# Credit_Bank
## 1. Mục đích báo cáo
Với vai trò là một chuyên gia phân tích rủi ro tín dụng tại Nova Bank – một tổ chức tài chính cung cấp các khoản vay cá nhân, y tế, giáo dục và kinh doanh trên khắp Hoa Kỳ, Vương quốc Anh và Canada. Nova Bank mong muốn việc cho vay trở nên công bằng và dễ tiếp cận hơn, đồng thời vẫn bảo vệ ngân hàng trước những rủi ro không cần thiết.
Thách thức chính là tìm ra sự cân bằng phù hợp. Nếu Nova Bank phê duyệt quá nhiều khoản vay rủi ro cao, họ sẽ mất tiền. Nếu quá khắt khe, họ sẽ bỏ lỡ những khách hàng tiềm năng. Bằng cách nhìn vào dữ liệu, nhiệm vụ của bạn là giúp ngân hàng hiểu rõ ai là người có xu hướng nợ quá hạn (default), tại sao họ lại làm vậy, và làm thế nào để các quyết định cho vay trở nên đáng tin cậy hơn.

## 2. Mô tả chi tiết dữ liệu

### a. Nguồn dữ liệu
* **Tệp tin:** `Credit_Risk_Dataset.xlsx`
* **Phạm vi:** Dữ liệu khách hàng tại Hoa Kỳ, Vương quốc Anh và Canada.

### b. Danh mục các biến số (Data Dictionary)

| Nhóm thông tin | Tên cột (Field Name) | Mô tả chi tiết |
| :--- | :--- | :--- |
| **Định danh & Nhân khẩu** | `Client_ID` | Mã định danh duy nhất cho mỗi khách hàng |
| | `person_age` | Tuổi của người nộp đơn (năm) |
| | `gender` | Giới tính (Nam/Nữ) |
| | `marital_status` | Tình trạng hôn nhân (Độc thân/Kết hôn/Ly hôn/Góa phụ) |
| | `education_level` | Trình độ học vấn (Trung học/Cử nhân/Thạc sĩ/Tiến sĩ) |
| **Nghề nghiệp & Thu nhập** | `person_income` | Thu nhập hàng năm (USD) |
| | `person_emp_length` | Thâm niên làm việc (số năm) |
| | `employment_type` | Loại hình công việc (Toàn thời gian/Bán thời gian/Tự doanh/Thất nghiệp) |
| **Nơi cư trú** | `person_home_ownership` | Tình trạng sở hữu nhà (Thuê/Chính chủ/Thế chấp) |
| | `country`, `state`, `city` | Quốc gia, Bang và Thành phố cư trú |
| | `city_latitude`, `city_longitude` | Tọa độ địa lý (Vĩ độ và Kinh độ) của thành phố |
| **Chi tiết khoản vay** | `loan_intent` | Mục đích vay (Cá nhân, Y tế, Giáo dục, Kinh doanh...) |
| | `loan_grade` | Xếp hạng tín dụng của khoản vay (từ A đến G) |
| | `loan_amnt` | Số tiền đề nghị vay (USD) |
| | `loan_int_rate` | Lãi suất khoản vay (%) |
| | `loan_status` | Trạng thái thanh toán (**0**: Không nợ xấu, **1**: Nợ xấu/Vỡ nợ) |
| | `loan_term_months` | Thời hạn vay (12, 24, 36, 60 tháng) |
| **Chỉ số tài chính** | `loan_percent_income` | Tỷ lệ số tiền trả nợ trên tổng thu nhập |
| | `loan_to_income_ratio` | Tỷ lệ số tiền vay trên tổng thu nhập |
| | `other_debt` | Các khoản nợ giả lập khác khách hàng đang có (USD) |
| | `debt_to_income_ratio` | Tỷ lệ tổng nợ trên thu nhập (DTI) |
| **Lịch sử tín dụng** | `open_accounts` | Số lượng tài khoản tín dụng đang mở |
| | `credit_utilization_ratio` | Tỷ lệ sử dụng hạn mức tín dụng (0–1) |
| | `cb_person_default_on_file` | Khách hàng đã từng có lịch sử nợ xấu trước đây chưa (Y/N) |
| | `cb_person_cred_hist_length` | Chiều dài lịch sử tín dụng (số năm) |
| | `past_delinquencies` | Số lần quá hạn thanh toán/vi phạm trong quá khứ |
## 3. Modeling
<img width="855" height="524" alt="image" src="https://github.com/user-attachments/assets/569c7656-366b-4946-9860-7128e597e18f" />

## 4. Thiết kế báo cáo
Credit_risk_report.pdf
https://github.com/LoNeiY511/Credit_Bank/blob/main/Credit_Risk_Report.pdf

## 📊 Phân tích Rủi ro Tín dụng & Xây dựng Dashboard (Power BI)

### **Tổng quan dự án**
Phân tích tập dữ liệu của hơn **32.000 khách hàng** với tổng dư nợ **312 triệu USD**, nhằm xác định các yếu tố dẫn đến nợ xấu và xây dựng giải pháp tối ưu hóa danh mục cho vay.

### **Các kết quả chính**
* **Xác định tỷ lệ nợ xấu (Default Rate):** Chạm mức **~22%**.
* **Phân tích nhân tố ảnh hưởng:** Xác định 4 biến số có tác động lớn nhất đến rủi ro: **Thu nhập (Income)**, **Xếp hạng tín dụng (Credit Grade)**, **Tình trạng nhà ở (person_home_ownership)** và **Tỷ lệ nợ/thu nhập (DTI)**.


### **Đề xuất cải tiến chính sách**
Dựa trên kết quả phân tích, các thay đổi chiến lược đã được đề xuất để giảm thiểu rủi ro hệ thống:
* **Kiểm soát ngưỡng an toàn:** Giới hạn tỷ lệ vay/thu nhập dưới **0.4** để giảm thiểu xác suất vỡ nợ.
* **Siết chặt điều kiện:** Áp dụng tiêu chuẩn khắt khe hơn đối với phân khúc khách hàng có thu nhập thấp (**<30K USD/năm**).
* **Tối ưu danh mục:** Loại bỏ cấp tín dụng cho nhóm khách hàng thuộc phân loại rủi ro cao (**Grade D đến G**).

### **Trực quan hóa dữ liệu**
Xây dựng Dashboard đa chiều hỗ trợ ra quyết định kinh doanh dựa trên các khía cạnh:
* **Nhân khẩu học:** Độ tuổi, khu vực, tình trạng nhà ở.
* **Tài chính:** Thu nhập, tổng dư nợ, mục đích vay vốn.
* **Lịch sử tín dụng:** Thời gian vay, các khoản nợ quá hạn trong quá khứ.

---
*Công cụ sử dụng: Power BI (DAX, Power Query)


