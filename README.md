# Window-Datathon-2026
Bài dự thi Datathon - Đội Window: Phân tích hành vi khách hàng và xây dựng mô hình dự báo tăng trưởng doanh thu.

Đội thi: Window

Thành viên: Yến Phương, Anh Thư
## Giới thiệu dự án
Dự án tập trung nghiên cứu phân khúc và hành vi khách hàng của doanh nghiệp dựa trên dữ liệu giai đoạn 2012-2022. Chúng tôi kết hợp phân tích dữ liệu để đưa ra các chiến lược kinh doanh và xây dựng mô hình dự báo doanh thu nhằm tối ưu hóa quyết định quản trị.

Kết quả nổi bật:
- Insight khách hàng: Xác định nhóm 25-44 tuổi là tệp chủ lực; đề xuất tái định vị thương hiệu.
- Mô hình dự báo: Hệ thống Ensemble (kết hợp LightGBM, Ridge Regression và Prophet) đạt độ chính xác cao với $R^2 \approx 0.83$ (LightGBM).

## Cấu trúc bài nộp

Dưới đây là các file chính trong dự án:

1. Window_datathon_2.ipynb:
- Chứa toàn bộ mã nguồn xử lý dữ liệu và trực quan hóa dữ liệu (Data Visualization).
- Các biểu đồ về nhân khẩu học, hành vi theo mùa vụ và hiệu quả các kênh marketing.

2. Window_datathon_3.py:
- File Python chứa mã nguồn xây dựng model dự báo.
- Triển khai thuật toán Ensemble 3 tầng để dự báo doanh thu dài hạn và ngắn hạn.

3. submission.csv
- File chứa kết quả dự báo doanh thu cuối cùng sinh ra từ mô hình.
- Đây là file dùng để hệ thống
 
4. Datathon2026: Đội_thi_Window.pdf:
- Báo cáo tổng hợp chính thức.
- Nội dung bao gồm: Phân tích khách hàng, kết quả trực quan hóa, giải thích mô hình dự báo và các đề xuất chiến lược kinh doanh.

## Hướng dẫn chạy lại kết quả
1. Cài đặt các thư viện cần thiết:

```
pip install pandas numpy matplotlib seaborn lightgbm scikit-learn prophet
```
2. Chạy file notebook Window_datathon_2.ipynb để xem các phân tích trực quan.
3. Chạy file Window_datathon_3.py để thực hiện huấn luyện mô hình.
```
python Window_datathon_3.py
```
*(Lưu ý: Sau khi chạy xong script này, file kết quả submission.csv sẽ tự động được tạo ra/cập nhật).*
