# 🎓 Student Performance Analysis Project

> **Mục tiêu:** Phân tích toàn diện các yếu tố ảnh hưởng đến kết quả học tập của học sinh, từ đó đề xuất các giải pháp tối ưu hóa hiệu quả giáo dục dựa trên dữ liệu.

<div align="center">

<a href="https://www.kaggle.com/datasets/kundanbedmutha/student-performance-dataset">
  <img src="https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" alt="Kaggle"/>
</a>
&nbsp;
<a href="LINK_GOOGLE_COLAB_CUA_BAN">
  <img src="https://img.shields.io/badge/Notebook-Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" alt="Google Colab"/>
</a>

</div>

---

## 📊 Data Dictionary (Từ điển dữ liệu)

Tập dữ liệu bao gồm các biến số quan trọng xoay quanh môi trường học tập và sinh hoạt của học sinh.

| Tên biến (Variable) | Ý nghĩa (Description) | Loại biến (Type) |
| :--- | :--- | :--- |
| **School Type** | Loại hình trường học (Công/Tư) | Categorical |
| **Gender** | Giới tính học sinh | Categorical |
| **Overall Score** | Điểm tổng kết trung bình | Numerical |
| **Math / Science / English Score** | Điểm thành phần các môn | Numerical |
| **Final Grade** | Xếp loại học lực cuối kỳ | Categorical (Ordinal) |
| **Study Hours** | Tổng giờ học tự học | Numerical |
| **Attendance** | Tỉ lệ chuyên cần | Numerical (%) |
| **Study Method** | Phương pháp học tập chính | Categorical |
| **Parent Education** | Trình độ học vấn phụ huynh | Categorical (Ordinal) |
| **Travel Time** | Thời gian di chuyển đến trường | Numerical |
| **Internet Access** | Có kết nối Internet hay không | Binary (Yes/No) |
| **Extra Activities** | Tham gia hoạt động ngoại khóa | Binary (Yes/No) |

---

## 🚀 Analytical Questions (Bộ câu hỏi phân tích)

Dự án tập trung giải quyết 20 câu hỏi trọng tâm, được chia thành 4 giai đoạn phân tích chính:

### I. Exploratory Data Analysis (EDA) & Distribution
*Khám phá cấu trúc dữ liệu và các phân phối cơ bản.*

1. **Demographic Distribution:** Cơ cấu học sinh phân bố như thế nào theo hai yếu tố `School Type` và `Gender`?
2. **Normality Test:** Phổ phân phối của `Overall Score` có tuân theo phân phối chuẩn (Normal Distribution) không? (Kiểm chứng bằng Histogram & Shapiro-Wilk test).
3. **Subject Comparison:** So sánh phân phối điểm giữa `Math`, `Science` và `English`. Môn nào có phổ điểm thấp nhất/biến động nhất?
4. **Grade Proportion:** Tỉ lệ phân bổ các mức `Final Grade` (A, B, C...) trong toàn trường hiện ra sao?
5. **Dispersion by Gender:** So sánh độ lệch chuẩn (Standard Deviation) của điểm số giữa Nam và Nữ để đánh giá tính ổn định trong kết quả học tập.

### II. Correlation & Factors Analysis
*Xác định các mối quan hệ tuyến tính và nhân quả giữa các biến.*

6. **Time vs. Performance:** Phân tích mối tương quan (Correlation) giữa `Study Hours` và `Overall Score`. (Hướng, cường độ và ý nghĩa thống kê Pearson/Spearman).
7. **Impact of Attendance:** `Attendance` ảnh hưởng cụ thể như thế nào tới phân bố `Overall Score`? (Sử dụng Scatter plot hoặc Regression line).
8. **Study Method Efficiency:** Đánh giá hiệu quả của từng `Study Method` đối với từng môn học riêng biệt (Toán, Khoa học, Anh văn).
9. **Correlation Matrix:** Xây dựng ma trận tương quan (Heatmap) giữa các biến định lượng để tìm ra "Feature" ảnh hưởng mạnh nhất đến kết quả học tập.
10. **Parental Influence:** Xu hướng thay đổi của `Overall Score` khi trình độ học vấn cha mẹ tăng dần (từ *No Formal* đến *PhD*)?

### III. Segmentation & Comparative Analysis
*So sánh sự khác biệt giữa các nhóm đối tượng đặc thù.*

11. **Digital Gap:** Với nhóm đi học xa (`Travel Time > 60 min`), việc có `Internet Access` có giúp cải thiện điểm số so với nhóm không có không?
12. **Extracurricular Balance:** Nhóm tham gia `Extra Activities` có điểm trung bình cao hơn hay thấp hơn nhóm không tham gia? (Kiểm định t-test).
13. **School Environment:** So sánh phân bố `Math Score` giữa Trường Công (Public) và Trường Tư (Private).
14. **Gender & Science:** Với cùng một `Study Method`, hiệu quả điểm `Science Score` giữa Nam và Nữ có sự khác biệt thống kê không?
15. **Elite Profiling:** So sánh đặc điểm hành vi (`Study Hours`, `Attendance`) của nhóm **Top 1%** học sinh xuất sắc nhất giữa hai loại hình trường.

### IV. Advanced Insights & Modeling
*Phân tích chuyên sâu, phát hiện bất thường và dự báo.*

16. **Feature Engineering (Efficiency Index):** Tạo chỉ số `Efficiency = Overall Score / Study Hours`. Nhóm độ tuổi (`Age`) nào có hiệu suất học tập tốt nhất?
17. **Anomaly Detection (Low Efficiency):** Phân tích nhóm "Nỗ lực ảo" (Top 25% Study Hours nhưng Bottom 25% Score). Nguyên nhân do phương pháp học sai hay chuyên cần thấp?
18. **Density Analysis:** Sử dụng Heatmap 2D để trực quan hóa vùng mật độ học sinh đạt **Điểm A** theo hai trục: `Attendance` vs `Study Hours`.
19. **Profile Contrast:** So sánh hồ sơ đặc trưng (Radar Chart) giữa nhóm Thủ khoa và nhóm Điểm thấp nhất. Yếu tố nào tạo ra khoảng cách lớn nhất?
20. **Predictive Modeling:** Xây dựng mô hình **Linear Regression** dự đoán `Overall Score`.
    * *Yêu cầu:* Feature Selection, đánh giá mô hình (R-squared, RMSE) và kiểm tra đa cộng tuyến.

---

### 🛠 Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SciPy.

---
<div align="center">
  <i>Project by Trần Phú Dinh, <a href="trhlow">, <a href="@baokhuu965-alt"></i>
</div>
