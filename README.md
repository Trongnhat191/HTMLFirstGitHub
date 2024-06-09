# Games in ESP32 Arduino

![Games in ESP32](https://github.com/HungHyperX/GamesInESP32-BTLNhung/assets/131465286/536e97e5-35ec-43c5-ac53-97970961aac3)


## Giới thiệu
&emsp;Đề tài triển khai trò chơi Flappy Bird và Dino Run trên ESP32 bằng cách sử dụng kiến trúc Arduino. Trò chơi được thiết kế để chạy trên màn hình SSD1306 Oled 1,3 inch, mang lại trải nghiệm thú vị và tương tác trên nền tảng ESP32.

Các tính năng chính bao gồm : 
- Điều khiển : Người chơi sử dụng nút bấm hoặc cảm biến đo khoảng cách để khiến nhân vật nhảy lên 
- Màn hình OLED : trò chơi được thiết kế để hiển thị trên màn hình OLED 1.3 inches. 
- Chuyển trò chơi : Có thể lựa chọn giữa 2 trò chơi Flappy Bird và Dino 
- Điểm cao : Lưu High Score của người chơi và điểm cao có thể được Reset

## Hướng dẫn và chơi

1. Clone repository về máy.

2. Mở project trên Arduino IDE

3. Cài đặt các thư viện cần thiết bằng Arduino Library Manager

4. Cấu hình dự án bằng cách chọn board và cổng thích hợp.

5. Tải lên ESP32.

6. Chọn 1 trong 2 game: Flappy Bird hoặc Dino Run

7. Điều khiển chim  hoặc khủng long bằng cách sử dụng các nút hoặc cảm biến được chỉ định.

8. Cố gắng vượt qua các đường ống hoặc cây xương rồng và ghi càng nhiều điểm càng tốt.

## Danh sách linh kiện

- ESP32 Development Board.
- Màn hình SSD1306 Oled tương thích với ESP32.
- 2 Nút bấm
- Còi
- Đèn LED và điện trở
- Cảm biến khoảng cách

## Sơ đồ nguyên lý

<ảnh>

- Màn hình của SH1106 nối với ESP 32 (SCL nối với chân 22, SDA nối với chân 21 của ESP32).
- Nút bấm thứ nhất nối với chân 23, nút bấm thứ hai nối với chân 27.
- Cảm biến đo khoảng cách: chân TRIG nối với chân 33, chân ECHO nối với chân 32 của ESP32.
- Còi có một chân nối với chân 18 của ESP32, chân còn lại nối đất.
- Đèn led thứ nhất nối với chân 5, đèn led thứ hai nối với chân 26 của ESP32, chân còn lại nối đất.

## Thư viện cài đặt
- [ThingPulse OLED SSD1306](https://github.com/ThingPulse/esp8266-oled-ssd1306.git): SSD1306 Oled display library for ESP8266 and ESP32.
- [Preferences](https://github.com/vshymanskyy/Preferences): Library to store the high score in the internal flash filesystem of ESP32.

## Thiết kế phần mềm


## Nhóm sinh viên thực hiện
- Nguyễn Đình Tuấn Đạt - MSSV: 20215562
- Phạm Lưu Minh Hùng - MSSV: 20215586
- Phạm Anh Tuấn - MSSV: 20215661
- Đỗ Đào Phúc - MSSV: 20210684
- Nguyễn Trọng Nhật - MSSV: 20215625

## Nguồn tham khảo
