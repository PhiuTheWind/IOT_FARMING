# 🌐 IoT Project

## 📖 Giới thiệu

Dự án **IoT (Internet of Things)** này được xây dựng nhằm cung cấp một
hệ thống kết nối, thu thập và xử lý dữ liệu từ nhiều thiết bị thông
minh. Hệ thống giúp giám sát, điều khiển và phân tích dữ liệu theo thời
gian thực, ứng dụng trong các lĩnh vực như **nhà thông minh, nông nghiệp
thông minh, công nghiệp 4.0** và nhiều kịch bản IoT khác.

Dự án tập trung vào: - Kiến trúc
hệ thống IoT từ **thiết bị cảm biến → gateway → nền tảng điện toán đám
mây → ứng dụng người dùng**. 
- Tích hợp nhiều module khác nhau để thu thập và truyền dữ liệu hiệu
quả. 
- Cơ chế lưu trữ, xử lý và hiển thị dữ liệu theo thời gian thực.

------------------------------------------------------------------------

## ⚙️ Tính năng chính

-   **Kết nối thiết bị IoT**: Hỗ trợ nhiều loại cảm biến và bộ truyền
    tín hiệu. 
-   **Truyền dữ liệu qua mạng**: Sử dụng giao thức MQTT/HTTP. 
-   **Lưu trữ dữ liệu trên cloud**: Cho phép quản lý và phân tích dữ
    liệu tập trung. 
-   **Ứng dụng giám sát**: Hiển thị dữ liệu trực quan qua dashboard
    CoreIOT Platform. 
-   **Tự động hóa**: Kích hoạt hành động dựa trên điều kiện (ví dụ: bật
    quạt khi nhiệt độ cao).

------------------------------------------------------------------------

## 🏗️ Kiến trúc hệ thống
1. **Thiết bị cảm biến**: Thu thập thông tin từ môi trường (nhiệt độ, độ
ẩm, ánh sáng, v.v.). 
2. **Gateway**: Xử lý sơ bộ và gửi dữ liệu lên server/cloud. 
3. **Cloud Server**: Lưu trữ, phân tích và chạy thuật toán. 
4. **Ứng dụng người dùng**: Giao diện hiển thị dữ liệu và cho phép điều
khiển từ xa.

------------------------------------------------------------------------

## 💡 Các Ứng dụng Nổi Bật

### 🌱 2.1 Smart Farm (Yolo:Farm)

Nông nghiệp là trụ cột cơ bản của nền kinh tế Việt Nam, mang lại sinh kế
cho hàng triệu lao động nông thôn. Tuy nhiên, ngành này đang đối mặt với
nhiều thách thức từ biến đổi khí hậu: mực nước biển dâng, lũ lụt, hạn
hán, xâm nhập mặn và thời tiết thất thường. Những yếu tố này ảnh hưởng
nghiêm trọng đến phương pháp canh tác truyền thống vốn phụ thuộc nhiều
vào lao động thủ công, gây ra **kém hiệu quả, chi phí cao và năng suất
thấp**.

Để giải quyết, dự án giới thiệu **Yolo:Farm**, một mô hình nông trại
thông minh quy mô nhỏ, tích hợp **tự động hóa, IoT và trí tuệ nhân tạo
(AI)** vào nông nghiệp hiện đại. Mục tiêu của Yolo:Farm: 
- Nâng cao năng suất. 
- Tối ưu hóa quản lý tài nguyên. 
- Giảm sự phụ thuộc vào lao động thủ công. 
- Tăng tính bền vững, thích ứng tốt hơn với biến đổi khí hậu.

Dự án này là minh chứng thực tiễn cho tiềm năng của **Nông nghiệp 4.0**,
hướng tới một nền nông nghiệp hiện đại và bền vững hơn.

### 🤖 2.2 AIoT (Artificial Intelligence of Things)

-   **AIoT** là sự kết hợp giữa **Trí tuệ nhân tạo (AI)** và **Internet
    of Things (IoT)**, cho phép thiết bị không chỉ thu thập dữ liệu mà
    còn **xử lý và học hỏi từ dữ liệu đó theo thời gian thực**. 
-   Khi ứng dụng vào nông trại thông minh, AIoT giúp tạo ra một **hệ
    sinh thái canh tác thông minh** nhờ khả năng:
    -   Phát hiện sớm bệnh hại cây trồng. 
    -   Dự báo tác động của thời tiết. 
    -   Hỗ trợ ra quyết định và quản lý tài nguyên một cách chủ động. 
-   Tích hợp AIoT trong Yolo:Farm mang lại **năng suất cao hơn, giảm chi
    phí, tăng hiệu quả và giảm lãng phí**.

------------------------------------------------------------------------

## 💻 Yêu cầu hệ thống

-   **Phần cứng**: YoloUno, cảm biến nhiệt độ, độ ẩm... 
-   **Phần mềm**:
    -   PlatformIO IDE 
    -   MQTT broker (Eclipse Mosquitto) 
-   **Dashboard**: [CoreIOT Platform](https://coreiot.io/) 
-   **Cloud/Server**: AWS IoT, Google Cloud IoT Core hoặc server riêng.

------------------------------------------------------------------------

## 🚀 Cài đặt & Sử dụng

1.  **Clone repo**

    ``` bash
    git clone https://github.com/<username>/<repository>.git
    cd <repository>
    ```

2.  **Mở project bằng PlatformIO IDE**

    -   Import project vào PlatformIO IDE. 
    -   Cài đặt các thư viện cần thiết theo `platformio.ini`.

3.  **Cấu hình kết nối**

    -   Chỉnh sửa file `config.json` để khai báo thông tin MQTT broker
        và cloud server.

4.  **Chạy hệ thống**

    -   Upload firmware từ PlatformIO IDE lên YoloUno. 
    -   Khởi chạy hệ thống và giám sát dữ liệu qua [CoreIOT
        Platform](https://coreiot.io/).

------------------------------------------------------------------------

## 📌 Hướng phát triển

-   Tích hợp AI để phân tích dữ liệu cảm biến. 
-   Bổ sung tính năng bảo mật nâng cao. 
-   Tối ưu giao diện người dùng (UI/UX).
