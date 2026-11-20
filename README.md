# GIỚI THIỆU BÀI THỰC HÀNH

Trong bài thực hành này, em tiến hành tìm hiểu và xây dựng hệ thống đồng hồ bấm giờ sử dụng vi điều khiển ESP32 kết hợp với màn hình LCD1602 giao tiếp I2C và hai nút nhấn điều khiển. Đây là bài thực hành giúp vận dụng kiến thức về lập trình vi điều khiển, giao tiếp I2C, xử lý tín hiệu đầu vào từ nút nhấn và quản lý thời gian trong hệ thống nhúng.

Hệ thống được thiết kế với hai chức năng điều khiển chính. Nút START/PAUSE dùng để bắt đầu, tạm dừng hoặc tiếp tục quá trình đếm thời gian. Nút RESET dùng để đưa đồng hồ trở về trạng thái ban đầu. Thời gian được tính toán bằng hàm `millis()` của Arduino và hiển thị trực tiếp trên màn hình LCD1602 theo định dạng phút và giây.

Thông qua bài thực hành, em có thể hiểu rõ hơn cách kết nối và điều khiển các thiết bị ngoại vi với ESP32, cách sử dụng giao tiếp I2C để hiển thị dữ liệu trên LCD, cũng như cách xử lý nút nhấn và chống dội phím. Đặc biệt, việc sử dụng `millis()` thay cho hàm `delay()` giúp chương trình hoạt động liên tục, hạn chế tình trạng bị ngắt quãng trong quá trình xử lý.

Qua đó, bài thực hành giúp củng cố kiến thức lý thuyết và nâng cao kỹ năng thiết kế, lập trình, mô phỏng một hệ thống nhúng có khả năng đo và hiển thị thời gian thực tế.
