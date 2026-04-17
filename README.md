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

### Phân tích dữ liệu hơn 32K khách hàng với tổng dư nợ 312M, xây dựng dashboard đánh giá rủi ro tín dụng bằng Power BI 
### Xác định tỷ lệ vỡ nợ ~22% và các yếu tố ảnh hưởng chính: thu nhập, xếp hạng tín dụng, tỷ lệ vay/thu nhập 
### Phát hiện bất cập trong hệ thống chấm điểm: nhóm A, B vẫn có tỷ lệ nợ xấu cao (~10–16%) 
### Đề xuất cải tiến chính sách tín dụng: 
### •	Giới hạn tỷ lệ vay/thu nhập < 0.4 để giảm rủi ro vỡ nợ 
### •	Siết chặt cho vay với nhóm thu nhập <30K 
### •	Loại bỏ cấp tín dụng cho nhóm rủi ro cao (D–G) 
### Trực quan hóa dữ liệu theo nhiều chiều: nhân khẩu học, tài chính, lịch sử tín dụng giúp hỗ trợ ra quyết định



