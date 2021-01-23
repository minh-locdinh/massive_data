**MapReduce**

MapReduce được thiết kế bởi Google như 1 mô hình lập trình xử lý tập dữ liệu lớn song song, thuật toán được phân tán trên 1 cụm. 
Mặc dù, MapReduce ban đầu là công nghệ độc quyền của Google, nó đã trở thành thuật ngữ tổng quát hóa trong thời gian gần đây.


MapReduce gồm các thủ tục: 1 Map() và 1 Reduce(). 
Thủ tục Map() lọc (filter) và phân loại (sort) trên dữ liệu trong khi thủ tục Reduce() thực hiện tổng hợp dữ liệu. 
Mô hình này dựa tre7m các khái niệm biến đổi của bản đồ và reduce các chức năng trong lập trình hướng chức năng. 
Thư viện thủ tục Map() và Reduce() được viết bằng nhiều ngôn ngữ. 
Cài đặt miễn phí, phổ biến nhất của MapReduce là Apache Hadoop.

![introduce](https://dinhnguyenngoc.files.wordpress.com/2014/07/what_is_mapreduce.png?w=768&h=465)

**Các thuận lợi của các thủ tục MapReduce**

Nền tảng MapReduce thường gồm các máy chủ phân tán và nó chạy nhiều tác vụ khác nhau song song. 
Có nhiều thành phần quản lý việc giao tiếp giữa các nodes khác nhau của dữ liệu và cung cấp tính sẵn sàng cao và mức độ chịu lỗi. 
Chương trình được viết theo chức năng MapReduce đợc tự động được phân tán và thực thi song song trên các máy chủ. 
Nền tảng MapReduce quan tâm cả chi tiết của phân vùng dữ liệu và thực thi quá trình xử lý trên máy chủ phân tán lúc chạy. 
Trong khi xử lý nếu có lỗi, nền tảng cung cấp tính sẵn sàng cao và các node khác thực hiện thay thế nhiệm vụ của node bị lỗi.

**Nền tảng MapReduce hoạt động như thế nào?**

Thủ tục Map()

Luôn có 1 master node trong hạ tầng để nhận đầu vào. Ngay sau master node là các sub-inputs / sub-problems. Các sub-problems được phân phối đến các worker nodes. Một worker node sau đó xử lý chúng. Một khi worker node hoàn thành xử lý với sub-problem, nó trả kết quả trở về master node.

Thủ tục Reduce()

Tất cả worker nodes trả kết quả của sub-problem đã gán cho chúng về master node. Master node thu thập kết quả và tổng hợp thành kết quả của vấn đề lớn (big problem) ban đầu đã được gán cho master node.

Nền tảng MapReduce thực hiện các thủ tục Map() và Reduce() ở trên song song và độc lập nhau. Tất cả thủ tục Map() có thể chạy song song và khi mỗi worker node hoàn thành tác vụ thì chúng gửi trở về master node. Thủ tục cụ thể này có thể rất hiệu quả khi nó được thực hiện trên một số lượng rất lớn dữ liệu (big data).

**Nền tảng MapReduce có 5 bước khác nhau:**

*Chuẩn bị dữ liệu đầu vào cho Map()
*Thực thi mã Map() được cung cấp bởi người dùng
*Trộn dữ liệu xuất của Map vào Reduce Processor
*Thực thi mã Reduce() được cung cấp bởi người dùng
*Tạo dữ liệu xuất cuối cùng

**Luồng dữ liệu (dataflow) của nền tảng MapReduce:**

*Input Reader
*Map Function
*Partition Function
*Compare Function
*Reduce Function
Output Writer



