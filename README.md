Nhằm phân loại khách hàng, ta sẽ dùng phương pháp RFM và K-Means.  RFM là phương pháp phân loại bằng các chỉ số Recency (khoảng thời gian từ lần giao dịch gần nhất, tính bằng ngày), Frequency (tổng số lần giao dịch) và Monetary (tổng giá trị giao dịch).  K-Means  là thuật toán dùng để nhóm các khách hàng thành k cụm. Và những khách hàng trong cùng một cụm sẽ có các đặc điểm tương tự nhau. Kết hợp hai phương pháp RFM và K-Means, ta sẽ phân loại khách hàng theo các cụm (loại) dựa trên các đặc điểm về Recency, Frequency và Monetary.
Tóm tắt model:

B1: Tính các chỉ số R-F-M của từng khách hàng

B2: Vẽ biểu đồ phân phối của R-F-M và kiểm tra dữ liệu có chuẩn chưa (Normal Distribution), nếu chuẩn thì sang bước 4

B3: Tiến hành chuẩn hóa dữ liệu bằng các hàm log, sqrt, boxcox

B4: Scale dữ liệu đã được chuẩn hoá

B5: Áp dụng dữ liệu đã được scale vào mô hình K-Mean, tìm k bằng phương pháp elbow

B6: Xác định cụm thích hợp của từng khách hàng

B7: Tìm giá trị trung bình của R-F-M trong từng cụm và xác định loại khách hàng.
	

