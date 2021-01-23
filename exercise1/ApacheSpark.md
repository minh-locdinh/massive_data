**Apache Spark**

Apache Spark là một open source cluster computing framework được phát triển sơ khởi vào năm
2009 bởi AMPLab tại đại học California, Berkeley.

Spark cho phép xây dựng và phân tích nhanh các mô hình dự đoán. Hơn nữa, nó còn cung cấp khả
năng truy xuất toàn bộ dữ liệu cùng lúc, nhờ vậy ta không cần phải lấy mẫu dữ liệu đòi hỏi bởi các ngôn ngữ lập trình như R.

Spark sử dụng API Resilient Distributed Dataset (RDD) để xử lý dữ liệu. Spark nhận được nhiều sự
hưởng ứng từ cộng đồng Big Data trên thế giới do cung cấp khả năng tính toán nhanh và nhiều thư
viện hữu ích đi kèm như Spark SQL (với kiểu dữ liệu DataFrames), Spark Streaming, MLlib
(machine learning: classification, regression, clustering, collaborative filtering, và dimensionality
reduction) và GraphX (tính toán song song trên dữ liệu đồ thị)

**Apache Spark có các tính năng đặc trưng sau đây:**

* Tốc độ: Spark có thể chạy trên cụm Hadoop và có thể chạy nhanh hơn 100 lần khi chạy trên
bộ nhớ RAM, và nhanh hơn 10 lần khi chạy trên ổ cứng. Bằng việc giảm số thao tác đọc nghi
lên đĩa cứng. Nó lưu trữ trực tiếp dữ liệu xử lý lên bộ nhớ.

* Hỗ trợ đa ngôn ngữ: Spark cung cấp các API có sẵn cho các ngôn ngữ Java, Scala, hoặc
Python. Do đó, bạn có thể viết các ứng dụng bằng nhiều các ngôn ngữ khác nhau. Spark đi
kèm 80 truy vấn tương tác mức cao.

* Phân tích nâng cao: Spark không chỉ hỗ trợ Map và Reduce, nó còn hỗ trợ truy vấn SQL, xử lý
theo Stream, học máy, và các thuật toán đồ thị (Graph)

**Các thành phần của Apache Spark**

![introduce](https://www.tutorialandexample.com/wp-content/uploads/2020/03/Apache-Spark-Components.png)

* Apache Spark Core: Spark Core là thành phần cốt lõi thực thi cho tác vụ cơ bản làm nền
tảng cho các chức năng khác. Nó cung cấp khảnăng tính toán trên bộ nhớ và dataset trong
bộ nhớ hệ thống lưu trữ ngoài.

* Spark SQL: Là một thành phần nằm trên Spark Core, nó cung cấp một sự ảo hóa mới cho dữ
liệu là SchemaRDD, hỗ trợ các dữ liệu có cấu trúc và bán cấu trúc.

* Spark Streaming: Cho phép thực hiện phân tích xử lý trực tuyến xử lý theo lô.

* MLlib (Machine Learning Library): MLlib là một nền tảng học máy phân tán bên trên Spark
do kiến trúc phân tán dựa trên bộ nhớ. Theo các so sánh benchmark Spark MLlib nhanh hơn
9 lần so với phiên bản chạy trên Hadoop (Apache Mahout).

* GrapX: Grapx là nền tảng xử lý đồ thị dựa trên Spark. Nó cung cấp các Api để diễn tả các
tính toán trong đồ thị bằng cách sử dụng Pregel Api.


