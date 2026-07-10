---
title: "Worklog Tuần 10"
date: 2026-06-22
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Objective of Worklog:

* :
* Hoàn thiện hệ thống vũ khí top-down với nhiều loại weapon khác nhau.
* Bổ sung hiệu ứng hình ảnh cho đòn đánh, Block, Parry và projectile.
* Tạo công cụ debug để dễ nhìn và tinh chỉnh hitbox, block direction và parry direction.
* Kiểm thử hoàn chỉnh cơ chế online trong Unity.
* Chuẩn bị bước đầu để build game và đưa server online lên AWS.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Hoàn thiện flow Lobby và Map Lobby<br> - Thiết kế luồng vào Boss Room<br> - Kiểm thử spawn Player online/offline<br> - Chuẩn bị scene BossRoom\_Minotaur | 22/06/2026 | 22/06/2026 | Unity Documentation, Netcode for GameObjects |
| 3 | - Setup Cinemachine camera cho top-down gameplay<br> - Cấu hình camera follow local player<br> - Thiết lập CameraBounds và xử lý lỗi Player bị đẩy ngoài map<br> - Kiểm tra camera trong cả offline và online mode | 23/06/2026 | 23/06/2026 | Unity Cinemachine Documentation |
| 4 | - Hoàn thiện hệ thống UI gameplay<br> - Liên kết Stats với Health, Mana và Poise UI<br> - Kiểm tra Weapon Pickup offline/online<br> - Sửa lỗi nhặt vũ khí và truyền sai WeaponData | 24/06/2026 | 24/06/2026 | Unity Documentation, Project source code |
| 5 | - Tối ưu NetworkPlayer và PlayerMove<br> - Kiểm thử nhiều client trong cùng LobbyScene<br> - Sửa lỗi NetworkManager và UnityTransport<br> - Kiểm thử người chơi online di chuyển, aim, đổi vũ khí và vào map | 25/06/2026 | 25/06/2026 | Netcode for GameObjects |
| 6 | - Hoàn thiện nhiều loại vũ khí: Sword, Spear, Bow, Staff<br> - Setup Spear với chuột trái combo 2 đòn và chuột phải Parry nhanh<br> - Setup Bow Rapid Fire/Burst Rapid Fire<br> - Setup Staff homing magic bolt và heal aura<br> - Bổ sung icon kỹ năng chuột trái/chuột phải cho WeaponData | 26/06/2026 | 26/06/2026 | Unity Documentation, Project source code |
| 7 | - Thiết kế hệ thống Slash Effect Prefab cho weapon<br> - Setup Shield Wave effect khi nhấn Block<br> - Setup Hold Pulse effect khi giữ Block<br> - Setup Spark effect chỉ khi Block hoặc Parry thành công<br> - Bổ sung projectile trail cho Arrow và Magic Bolt | 27/06/2026 | 27/06/2026 | Unity Documentation, Project source code |
| CN | - Tạo công cụ debug hitbox cho ActionHitBox<br> - Vẽ preview hướng Block và Parry trong Scene View<br> - Tinh chỉnh vùng đánh cho Sword, Spear và Shield<br> - Chuẩn bị kiến trúc AWS gồm EC2, Lambda Function URL và DynamoDB<br> - Bắt đầu xử lý build Linux Dedicated Server và kết nối SSH tới EC2 | 28/06/2026 | 28/06/2026 | AWS Documentation, Unity Dedicated Server Documentation |


### Kết quả đạt được tuần 10:

* Hoàn thiện hệ thống vũ khí top-down với nhiều loại weapon:
* Sword có combo, Block và Parry.
* Spear có chuột trái combo 2 đòn và chuột phải Parry nhanh, không hold Block.
* Bow có Rapid Fire và Burst Rapid Fire.
* Staff có homing magic bolt và kỹ năng hồi máu/buff.
* Bổ sung hệ thống icon kỹ năng cho WeaponData:
* Icon kỹ năng chuột trái.
* Icon kỹ năng chuột phải.
* Tên kỹ năng chính và kỹ năng phụ.
* Có thể hiển thị lên UI gameplay.
* Hoàn thiện hệ thống hiệu ứng hình ảnh cho combat:
* Slash Effect Prefab cho Sword.
* Stab Effect Prefab cho Spear.
* Wave Effect cho Shield khi nhấn Block.
* Hold Pulse Effect khi giữ Block.
* Spark Effect chỉ xuất hiện khi Block hoặc Parry thành công.
* Trail effect cho Arrow và Magic projectile.
* Tạo công cụ debug giúp dễ tinh chỉnh combat:
* Hiển thị ActionHitBox theo hướng aim.
* Hiển thị vùng đánh thật khi animation gọi AttackAction.
* Hiển thị Block Direction.
* Hiển thị Parry Direction.
* Giúp chỉnh tầm đánh và vùng đánh trực quan hơn trong Scene View.
* Kiểm thử online trong Unity đã hoạt động tốt:
* Host/Client có thể vào Lobby.
* Player online có thể di chuyển và aim đúng.
* Weapon hoạt động trong môi trường online.
* Boss room và Map Lobby đã sẵn sàng để tiếp tục test online.
* Chuẩn bị bước đầu cho triển khai AWS:
* Lựa chọn mô hình 3 dịch vụ: EC2, Lambda Function URL và DynamoDB.
* Chuẩn bị Unity Linux Dedicated Server.
* Tạo kế hoạch upload server build lên EC2.
* Xử lý lỗi quyền file PEM khi kết nối SSH từ Windows.


