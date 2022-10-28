# Classification-disease-leaf
1. Thông tin chung:
- Tên đề tài: Phát hiện và phân loại bệnh lá cây
- Chủ nhiệm đề tài: Đặng Thanh Hưng		Mã số SV: 18119018
- Lớp: 18161CLVT2B 			                       Khoa:	Đào tạo Chất lượng cao

2. Mục tiêu đề tài:

Thiết kế hệ thống nhận biết bệnh lá cây sử dụng phương pháp phân tích cấu trúc ảnh, thuật toán mạng học sâu để huấn luyện mô hình mạng học sâu. Trong đó tập dữ liệu là một số loại bệnh phổ biến để đánh giá kết quả của thuật toán được kiến nghị. Sau đó triển khai mô hình đã được huấn luyện lên ứng dụng di dộng để dự đóan bệnh và đưa ra đề xuất điều trị bệnh cho người dùng.

3.	Tính mới và sáng tạo:

Hiện nay đã có nhiều nghiên cứu về lĩnh vực ứng dụng xử lý ảnh để phát hiện sâu bệnh trên cây trồng nhưng hầu hết chỉ dừng lại ở mức phân loại và thống báo cho người dùng về tình trạng cây trồng để người dùng sớm phát hiện và kịp thời đưa ra hướng giải quyết. Chính vì thế đòi hỏi người dùng cần phải am hiểu và có nhiều kinh nghiệm trong lĩnh vực trồng trọt, nếu không có thể xảy ra trường hợp trị sai bệnh gây tốn kém và không đạt hiệu quả. Chính vì những lý do trên, nhóm tác giả quyết định thực hiện đề tài không chỉ phát hiện, phân loại bệnh mà còn đơn giản hóa việc tìm hướng giải quyết cho người dùng bằng việc xây dựng thêm phần đề xuất hướng điều trị cho người dùng ứng dụng trên điện thoại.

4. Kết quả nghiên cứu:

Tất cả các thí nghiệm được thực hiện bằng ngôn ngữ Python. Các loại lá được xem xét bao gồm 14 tập ảnh về các bệnh phổ biến, trong đó có 9 tập được lấy từ thư viện Kaggel và 5 tập ảnh thu được từ thực tế. Việc phân loại lần đầu tiên được thực hiện bằng mô hình noron tích chập CNN cho kết quả với độ chính xác là 86.54%. Độ chính xác được cải thiện lên 93.63% với thuật toán được đề xuất bằng phương pháp kết hợp việc xử lý ảnh đầu vào để trích xuất đặc trưng và loại bỏ những phần không cần thiết trong ảnh. Thực hiện kiểm thử trên gần 2800 ảnh từ tập dữ liệu kiểm, tỷ lệ dự đoán chính xác là 98%. Tuy nhiên độ chính xác của mô hình được đào tạo hơi thấp hơn đối với các lớp có số lượng hình ảnh thấp hơn trong tập dữ liệu huấn luyện, cụ thể hơn là các lớp ảnh tự thu thập từ thực tế như ở bệnh đốm lá của cây đậu biết, và bệnh lá úa vàng ở cây mồng tơi. Đối với các loại lá có chất lượng ảnh tốt như bệnh đốm vi khuẩn ở cây ớt độ chính xác khi dự đoán cao nhất có thể đạt được lên đến 100%, đối với một số loại lá khác độ chính xác khoảng từ 84,6% đối với lá cà chua bị bệnh nhện ve 2 đốm và lá cà chua khỏe lên đến 99,35% đối với các loại lá còn lại. Với các tham số sau khi huấn luyện của mô hình phân loại bệnh, nhóm tác giả đã triển khai bộ nhân dạng bệnh lá cây lên ứng dụng di động dưới dạng mô hình được chuyển đổi sang dạng tensorflow lite. Mô hình này được chạy bằng api của google cloud platform (GCP) có khả năng dự đoán bệnh bằng ảnh chụp từ điện thoại và đưa ra các thông tin đề xuất bệnh cho người dùng về tình trạng bệnh. Kết quả về quá trình dự đoán được trình bày trong mục 3.2.

5. Đóng góp về mặt giáo dục và đào tạo, kinh tế - xã hội, an ninh, quốc phòng và khả năng áp dụng của đề tài: 

Kết quả nghiên cứu của đề tài sẽ được hỗ trợ cho các nhà trồng trọt hoặc để nghiên cứu trong việc chuẩn đoán nhanh và chính xác các bệnh lá cây giúp tăng năng suất thu hoạch trong trồng trọt. Ngoài ra cũng có thể ứng dụng cho việc giảng dạy và giáo dục.
Sản phẩm của đề tài nghiên cứu là ứng dụng di động có thể cho người nông dân trực tiếp chăm sóc cây trồng sử sụng hoặc dùng trong các dịch vụ giám sát hộ để giám sát vườn cây và nghiên cứu các loại bệnh mới.
