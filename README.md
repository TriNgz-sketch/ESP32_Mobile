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
   
## Hướng dẫn cài đặt
1.  **(Trên máy tính) Tải folder AppProject về máy ,Mở Terminal(chế độ Admin) ,tải Node.js, cấp quyền ,update Expo lên SDK57 theo app,cd tới đường dẫn smart-farm trong folder,gõ lệnh "npm install" để tải thư viện và gõ lệnh"npx expo start" để khởi động ,nó sẽ hiện mã Qr và link URL**
2.  **(Trên điện thoại) Tải ứng dụng Expo Go trên Chplay hoặc IOS ,sau đó quét mã trên terminal để vào app,đăng ký tài khoản và có thể sử dụng**
