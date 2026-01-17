# TK_PTDL
# Bộ câu hỏi phân tích dữ liệu học sinh

Mục tiêu: Chuẩn hóa 20 câu hỏi phân tích để đưa lên GitHub. Mỗi câu được viết rõ ràng, ngắn gọn và dễ thực hiện trên tập dữ liệu có các biến chính: School Type, Gender, Overall Score, Math Score, Science Score, English Score, Final Grade, Study Hours, Attendance, Study Method, Age, Travel Time, Internet Access, Extra Activities, v.v.
Link bộ dataset: "https://www.kaggle.com/datasets/kundanbedmutha/student-performance-dataset"

## Danh sách biến chính (ví dụ)
- Loại trường — School Type
- Giới tính — Gender
- Điểm tổng kết — Overall Score
- Điểm Toán — Math Score
- Điểm Khoa học — Science Score
- Điểm Tiếng Anh — English Score
- Xếp loại học lực — Final Grade
- Giờ học / Thời gian học — Study Hours
- Chuyên cần — Attendance
- Phương pháp học — Study Method
- Tuổi — Age
- Thời gian đi học — Travel Time
- Có Internet — Internet Access
- Tham gia ngoại khóa — Extra Activities

---

### Câu hỏi phân tích (chuẩn hóa)

1. Cơ cấu học sinh phân bố như thế nào theo hai yếu tố Loại trường (School Type) và Giới tính (Gender)?
2. Phổ phân phối của Điểm tổng kết (Overall Score) có phù hợp với phân phối chuẩn hay không (kiểm tra bằng biểu đồ và kiểm định)?
3. So sánh điểm trung bình giữa ba môn Toán (Math Score), Khoa học (Science Score) và Tiếng Anh (English Score) để xác định môn có phổ điểm thấp nhất.
4. Tỉ lệ phân bổ của các mức xếp loại học lực (Final Grade) trong toàn trường hiện như thế nào?
5. Phân tích mối tương quan giữa Thời gian học (Study Hours) và Điểm tổng kết (Overall Score): hướng, cường độ và ý nghĩa thống kê.
6. Chuyên cần (Attendance) ảnh hưởng cụ thể như thế nào tới phân bố của Điểm tổng kết (Overall Score)?
7. Đánh giá hiệu quả của các Phương pháp học (Study Method) đối với từng môn: Toán, Khoa học và Tiếng Anh (so sánh trung bình và phân bố).
8. Xây dựng chỉ số Efficiency = Overall Score / Study Hours. Phân tích chỉ số này theo độ tuổi (Age) để xác định nhóm tuổi có hiệu quả tiếp thu tốt nhất (điểm cao nhưng thời gian học thấp).
9. So sánh độ lệch chuẩn (standard deviation) của điểm số giữa Nam và Nữ để xác định giới tính có kết quả học tập ổn định hơn.
10. Ma trận tương quan giữa các biến định lượng (Study Hours, Attendance, test component scores, Overall Score) cho thấy những cặp biến nào có mối liên hệ mạnh nhất?
11. Xu hướng thay đổi của Điểm tổng kết (Overall Score) khi mức trình độ học vấn của cha mẹ tăng dần theo thứ tự: No Formal < High School < Diploma < Graduate < Post Graduate < PhD.
12. Với nhóm học sinh đi học xa (Travel Time = ">60 min"), việc có kết nối Internet (Internet Access = Yes) có giúp cải thiện Điểm tổng kết (Overall Score) so với nhóm không có Internet không?
13. Nhóm học sinh tham gia hoạt động ngoại khóa (Extra Activities = Yes) có điểm trung bình Overall Score khác (thấp/hay cao) so với nhóm không tham gia không?
14. So sánh phân bố điểm Toán (Math Score) giữa hai loại trường: Trường Công và Trường Tư.
15. Với cùng một Phương pháp học (Study Method), so sánh hiệu quả điểm môn Khoa học (Science Score) giữa học sinh Nam và Nữ.
16. So sánh đặc điểm (Study Hours, Attendance) của nhóm top 1% học sinh xuất sắc nhất giữa Trường Công và Trường Tư.
17. Phân tích nhóm "Hiệu quả thấp": những học sinh thuộc top 25% về thời gian học (Study Hours cao) nhưng thuộc bottom 25% về Overall Score — nguyên nhân chủ yếu là do phương pháp học hay do chuyên cần?
18. Sử dụng biểu đồ nhiệt (heatmap) để trực quan hóa vùng dữ liệu có mật độ học sinh đạt Điểm A cao nhất theo hai trục: Chuyên cần (Attendance) và Giờ học (Study Hours).
19. So sánh hồ sơ đặc trưng giữa nhóm Thủ khoa (highest Overall Score) và nhóm Điểm thấp nhất (lowest Overall Score): yếu tố có khác biệt lớn nhất là gì?
20. Xây dựng và đánh giá mô hình Hồi quy tuyến tính (Linear Regression) để dự đoán Điểm tổng kết (Overall Score) dựa trên các biến có tương quan mạnh nhất (ví dụ: Attendance, Study Hours, component scores). Nêu các bước chọn biến, đánh giá hiệu năng và kiểm định giả thiết của mô hình.
