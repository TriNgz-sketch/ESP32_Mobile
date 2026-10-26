# Ứng dụng Di động - IoT Smart Farm & Crop Monitoring System
## Giới thiệu
Đây là mã nguồn ứng dụng di động (Mobile App) thuộc dự án **Ứng dụng Di động kết hợp với hệ thống nhúng ESP32 - Quản lý và Giám sát cây trồng**. Hệ thống hướng đến việc ứng dụng công nghệ IoT vào nông nghiệp, kết hợp khối phần cứng thu thập dữ liệu tại vườn và nền tảng di động để theo dõi liên tục trạng thái môi trường.

## Tính năng chính
*   **Giám sát thông số thời gian thực (Real-time Monitoring):** Cập nhật liên tục các dữ liệu truyền về từ hệ thống vi điều khiển:
    *   Nhiệt độ & Độ ẩm không khí (Cảm biến DHT22)
    *   Cường độ ánh sáng (Module quang trở LDR)
    *   Độ ẩm đất (Cảm biến điện dung V1.2)
*   **Đồng bộ dữ liệu đám mây:** Giao tiếp hai chiều với phần cứng ESP32 thông qua Firebase Realtime Database.
*   **Giao diện trực quan:** Theo dõi số liệu tức thời, vẽ biểu đồ lịch sử theo thời gian và hiển thị các cảnh báo khi thông số môi trường vượt ra khỏi ngưỡng thiết lập.

## Công nghệ & Thiết bị sử dụng
*   **Phát triển Ứng dụng:** React Native, Expo, TypeScript.
*   **Cơ sở dữ liệu (Backend):** Firebase (Realtime Database & Authentication).
*   **Khối vi điều khiển:** Kit ESP32 CP2102 30 Pin (tích hợp Wi-Fi).
*   
## Hướng dẫn cài đặt
1.  **Clone repository về máy tính:**
    ```bash
    git clone [https://github.com/TriNgz-sketch/Esp32_Mobile.git](https://github.com/TriNgz-sketch/Esp32_Mobile.git)
    cd Esp32_Mobile
    ```
2.  **Cài đặt các gói thư viện cần thiết:**
    ```bash
    npm install
    ```
3.  **Cấu hình kết nối Firebase:**
    Cập nhật thông tin `firebaseConfig` (API Key, Database URL, v.v.) vào mã nguồn để ứng dụng có thể kết nối với cơ sở dữ liệu.
4.  **Khởi chạy ứng dụng:**
    ```bash
    npx expo start
    ```
    *Quét mã QR bằng ứng dụng Expo Go trên điện thoại để trải nghiệm.*
