---

title: "Worklog Tuần 12"
date: 2026-07-06
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
-----------------------

### Objective of Worklog:

* Hoàn thiện việc kiểm thử gameplay online trong Unity trước khi chuyển sang giai đoạn triển khai online bên ngoài.
* Chuẩn bị quy trình triển khai AWS cho server multiplayer của game RoughLife.
* Build và cấu hình Unity Linux Dedicated Server để phục vụ việc host game trên cloud.
* Thiết kế hướng kiến trúc AWS ban đầu sử dụng EC2, Lambda Function URL và DynamoDB.
* Chuẩn hóa tài liệu dự án, worklog và báo cáo sự kiện để chuẩn bị cho phần nộp báo cáo.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                                                                                                                                        | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                          |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------ | --------------- | ------------------------------------------------------- |
| 2   | - Rà soát lại toàn bộ luồng gameplay online đã hoàn thiện trong Unity <br> - Kiểm tra Lobby, Map Lobby, Boss Room, di chuyển Player, aim và tương tác vũ khí <br> - Xác nhận hệ thống online đã sẵn sàng để test với server bên ngoài                                                                                                            | 06/07/2026   | 06/07/2026      | Unity Documentation, Netcode for GameObjects            |
| 3   | - Hoàn thiện các công cụ debug combat <br> - Kiểm tra ActionHitBox preview, Block Direction preview và Parry Direction preview <br> - Tinh chỉnh hitbox cho Sword, Spear, Shield, Bow và Staff <br> - Xác nhận cơ chế vũ khí hoạt động ổn định ở cả offline và online mode                                                                       | 07/07/2026   | 07/07/2026      | Unity Documentation, Project source code                |
| 4   | - Lên kế hoạch kiến trúc AWS cho RoughLife <br> - Chọn mô hình ban đầu gồm 3 dịch vụ: EC2, Lambda Function URL và DynamoDB <br> - Xác định luồng online: Client yêu cầu room code, nhận IP/port server và kết nối vào dedicated server <br> - Rà soát thêm các dịch vụ có thể mở rộng trong tương lai như S3, CloudFront, CloudWatch và GameLift | 08/07/2026   | 08/07/2026      | AWS Documentation, Unity Dedicated Server Documentation |
| 5   | - Chuẩn bị bản build Unity Linux Dedicated Server <br> - Tạo hoặc rà soát scene ServerBoot và logic khởi động server <br> - Cấu hình UnityTransport để sử dụng kết nối UDP <br> - Chuẩn bị Windows Client build để test với người chơi bên ngoài <br> - Bắt đầu cấu hình EC2 server, Security Group, SSH access và UDP port 7777                 | 09/07/2026   | 09/07/2026      | Unity Dedicated Server, AWS EC2 Documentation           |
| 6   | - Upload và kiểm thử quy trình chạy dedicated server build trên AWS EC2 <br> - Sửa lỗi quyền file PEM trên Windows khi dùng SSH/SCP <br> - Tiếp tục chuẩn bị Lambda Function URL và thiết kế DynamoDB room table <br> - Chỉnh sửa, dịch và đồng bộ lại worklog, event report để thống nhất tài liệu                                              | 10/07/2026   | 10/07/2026      | AWS EC2, AWS Lambda, DynamoDB, Project Documentation    |

### Kết quả đạt được tuần 12:

* Hoàn thành việc kiểm thử gameplay online trong Unity:

  * Host và Client có thể tham gia luồng online.
  * Player online có thể di chuyển và aim đúng.
  * Các loại vũ khí có thể sử dụng trong môi trường online.
  * Map Lobby và Boss Room đã sẵn sàng cho bước test với server bên ngoài.

* Hoàn thiện các công cụ hỗ trợ tinh chỉnh combat và weapon:

  * Có thể nhìn rõ ActionHitBox trong Scene View.
  * Có thể preview hướng Block.
  * Có thể preview hướng Parry.
  * Việc điều chỉnh vùng đánh cho từng loại vũ khí trở nên trực quan và dễ kiểm soát hơn.

* Chuẩn bị được mô hình triển khai AWS ban đầu cho RoughLife:

  * EC2 được dùng để host Unity Dedicated Server.
  * Lambda Function URL được định hướng làm Room API.
  * DynamoDB được dùng để lưu thông tin phòng tạm thời.
  * Client có thể nhận server address và port trước khi kết nối vào game server.

* Chuẩn bị quy trình triển khai Unity Dedicated Server:

  * Xác định hướng build Linux Dedicated Server.
  * Chuẩn bị hướng build Windows Client.
  * Rà soát cấu hình UnityTransport với UDP.
  * Lên kế hoạch cho luồng khởi động server và cấu hình port.

* Bắt đầu setup AWS EC2 server:

  * Tạo hoặc chuẩn bị môi trường EC2 server.
  * Rà soát yêu cầu Security Group.
  * Xác định UDP port 7777 cho traffic game.
  * Sử dụng SSH/SCP để upload và quản lý file server.

* Sửa được lỗi quan trọng khi kết nối AWS:

  * Xác định lỗi file PEM trên Windows có quyền truy cập quá mở.
  * Điều chỉnh quyền file PEM bằng lệnh permission trên Windows.
  * Chuẩn bị lại quy trình SSH/SCP để upload Linux server build.

* Cải thiện phần tài liệu dự án:

  * Chỉnh lại form các file worklog tiếng Việt cho đúng template.
  * Tạo bản tiếng Anh tương ứng cho các worklog.
  * Viết lại nội dung event report để khác biệt hơn nhưng vẫn giữ nguyên bố cục.
  * Chuẩn bị tài liệu phục vụ báo cáo và trình bày trên GitHub.

* Tổng kết tuần 12: Quá trình kiểm thử online trong Unity đã hoàn thành ổn định, hệ thống weapon và công cụ debug combat đã dễ sử dụng hơn, đồng thời dự án bắt đầu bước sang giai đoạn chuẩn bị triển khai server lên AWS để test online với người chơi bên ngoài.

