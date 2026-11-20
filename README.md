# BÀI THỰC HÀNH 2: ĐỒNG HỒ BẤM GIỜ SỬ DỤNG ESP32 VÀ LCD1602

## 1. Giới thiệu

Bài thực hành xây dựng mô hình đồng hồ bấm giờ sử dụng vi điều khiển ESP32 kết hợp với màn hình LCD1602 giao tiếp I2C và hai nút nhấn điều khiển.

Hệ thống cho phép người dùng bắt đầu, tạm dừng, tiếp tục và đặt lại thời gian thông qua các nút nhấn. Thời gian được tính toán bằng hàm `millis()` và hiển thị trên màn hình LCD theo định dạng phút:giây (MM:SS).

## 2. Linh kiện sử dụng

- ESP32 DevKit V1.
- Màn hình LCD1602 giao tiếp I2C.
- 2 nút nhấn (START/PAUSE và RESET).
- Dây kết nối.

## 3. Chức năng chính

- **START:** Bắt đầu đếm thời gian.
- **PAUSE:** Tạm dừng đồng hồ.
- **RESUME:** Tiếp tục đếm thời gian sau khi tạm dừng.
- **RESET:** Đưa thời gian về 00:00.
- **LCD1602:** Hiển thị thời gian và trạng thái hoạt động (RUNNING/PAUSED).

## 4. Kiến thức áp dụng

- Lập trình vi điều khiển ESP32.
- Giao tiếp I2C với màn hình LCD1602.
- Đọc và xử lý tín hiệu từ nút nhấn.
- Kỹ thuật chống dội nút nhấn (Debounce).
- Sử dụng hàm `millis()` để quản lý thời gian mà không cần dùng `delay()`.

## 5. Mục tiêu bài thực hành

Hiểu được cách kết nối và điều khiển các thiết bị ngoại vi bằng ESP32, đồng thời vận dụng kiến thức lập trình hệ thống nhúng để xây dựng một ứng dụng đồng hồ bấm giờ có khả năng hoạt động liên tục và hiển thị trạng thái trực quan.

## 6. Công cụ mô phỏng

- Wokwi Simulator.
- Arduino IDE / Wokwi Editor.
