# Credit_Bank
1. Mục đích báo cáo
Với vai trò là một chuyên gia phân tích rủi ro tín dụng tại Nova Bank – một tổ chức tài chính cung cấp các khoản vay cá nhân, y tế, giáo dục và kinh doanh trên khắp Hoa Kỳ, Vương quốc Anh và Canada. Nova Bank mong muốn việc cho vay trở nên công bằng và dễ tiếp cận hơn, đồng thời vẫn bảo vệ ngân hàng trước những rủi ro không cần thiết.
Thách thức chính là tìm ra sự cân bằng phù hợp. Nếu Nova Bank phê duyệt quá nhiều khoản vay rủi ro cao, họ sẽ mất tiền. Nếu quá khắt khe, họ sẽ bỏ lỡ những khách hàng tiềm năng. Bằng cách nhìn vào dữ liệu, nhiệm vụ của bạn là giúp ngân hàng hiểu rõ ai là người có xu hướng nợ quá hạn (default), tại sao họ lại làm vậy, và làm thế nào để các quyết định cho vay trở nên đáng tin cậy hơn.
2. Mô tả chi tiết dữ liệu
a. Nguồn dữ liệu
 Credit_Risk_Dataset.xlsx

b. Tổng quan dữ liệu
b.1. Thông tin định danh và Nhân khẩu học
Client_ID: Mã định danh duy nhất cho mỗi khách hàng.
person_age: Tuổi của người nộp đơn (năm).
gender: Giới tính (Nam/Nữ).
marital_status: Tình trạng hôn nhân (Độc thân, Kết hôn, Ly hôn, Góa phụ).
education_level: Trình độ học vấn (Trung học, Cử nhân, Thạc sĩ, Tiến sĩ).
b.2. Thông tin nghề nghiệp và Thu nhập
person_income: Thu nhập hàng năm (USD).
person_emp_length: Thâm niên làm việc (số năm).
employment_type: Loại hình công việc (Toàn thời gian, Bán thời gian, Tự doanh, Thất nghiệp).
b.3. Thông tin nơi cư trú
person_home_ownership: Tình trạng sở hữu nhà (Thuê, Chính chủ, Đang thế chấp).
country / state / city: Quốc gia, Bang/Tỉnh, Thành phố nơi cư trú.
city_latitude / city_longitude: Tọa độ địa lý (Vĩ độ và Kinh độ) của thành phố.
b.4. Chi tiết về khoản vay
loan_intent: Mục đích vay (Cá nhân, Y tế, Giáo dục, v.v.).
loan_grade: Xếp hạng tín dụng của khoản vay (từ A đến G).
loan_amnt: Số tiền đề nghị vay (USD).
loan_int_rate: Lãi suất vay (%).
loan_status: Trạng thái thanh toán (0 = không nợ xấu, 1 = nợ xấu/vỡ nợ).
loan_term_months: Thời hạn vay tính theo tháng (12, 24, 36, 60).
b.5. Chỉ số tài chính và Lịch sử tín dụng
loan_percent_income: Tỷ lệ số tiền trả nợ trên thu nhập.
loan_to_income_ratio: Tỷ lệ khoản vay chia cho thu nhập của người nộp đơn.
other_debt: Các khoản nợ giả lập khác mà khách hàng đang có (USD).
debt_to_income_ratio: Tỷ lệ tổng nợ trên thu nhập (DTI).
open_accounts: Số lượng tài khoản tín dụng đang mở.
credit_utilization_ratio: Tỷ lệ sử dụng hạn mức tín dụng (từ 0 đến 1).
cb_person_default_on_file: Khách hàng đã từng có lịch sử nợ xấu trước đây chưa (Có/Không).
cb_person_cred_hist_length: Chiều dài lịch sử tín dụng (số năm).
past_delinquencies: Số lần quá hạn thanh toán/vi phạm trong quá khứ.

3. Modeling
<img width="855" height="524" alt="image" src="https://github.com/user-attachments/assets/569c7656-366b-4946-9860-7128e597e18f" />

4. Thiết kế báo cáo
Credit_risk_report.pdf
https://github.com/LoNeiY511/Credit_Bank/blob/main/Credit_Risk_Report.pdf


