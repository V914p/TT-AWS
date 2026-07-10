---
title: "Báo cáo tuần 11"
date: 2026-07-05
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Objective of Worklog:

* Hoàn thiện các chức năng Online quan trọng cho game co-op TopDown Boss Fight.
* Tích hợp luồng tạo phòng, vào phòng và chuyển cảnh giữa Lobby Scene, Map Lobby và Boss Room.
* Xây dựng thêm Boss Phoenix theo hướng Bullet Hell, có nhiều trạng thái và kỹ năng khác nhau.
* Hoàn thiện cơ chế kết thúc Boss Room, bao gồm thoát về Map Lobby, kiểm tra toàn bộ Player chết và spawn phần thưởng sau khi đánh bại Boss.
* Nâng cấp hệ thống vũ khí, phần thưởng và kỹ năng hỗ trợ cho Player.

### Công việc thực hiện trong tuần:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu / Ghi chú |
| --- | --- | --- | --- | --- |
| 2 | - Tiếp tục hoàn thiện luồng Online cho game. <br> - Kiểm tra lại Lobby Scene để Player có thể tạo phòng, nhập mã phòng và chuẩn bị vào Map Lobby. <br> - Dọn dẹp các object test trong Lobby Scene để chỉ giữ lại các thành phần cần thiết cho Online AWS. <br> - Điều chỉnh luồng Online để khi tạo room, Player không bị chuyển ngay vào Map Lobby mà có thể chờ người chơi khác tham gia. | 29/06/2026 | 29/06/2026 | Unity Netcode, AWS Room API |
| 3 | - Phân tích lại Core System để xây dựng cơ chế Revive cho Player. <br> - Thiết kế trạng thái Player bị gục, thanh máu bleedout giảm dần theo thời gian và cơ chế đồng đội đứng gần để hồi sinh. <br> - Đảm bảo cơ chế Revive có thể dùng cho Online nhưng không làm ảnh hưởng đến Player Offline. <br> - Kiểm tra lại luồng chết của Player khi vào Boss Room. | 30/06/2026 | 30/06/2026 | Core System, Stats, Revive System |
| 4 | - Bắt đầu xây dựng Boss Phoenix mới cho game. <br> - Thiết kế Phoenix theo hướng Bullet Hell với các trạng thái Fly State, Ground State, AOE Skill, Totem Skill, Fire Line Skill và Phase 2. <br> - Tạo các prefab hỗ trợ như Phoenix Bullet Totem, Phoenix Bullet Projectile và Phoenix Fire Line Hazard. <br> - Xử lý các lỗi phát sinh khi kết hợp Phoenix với State Machine và Core System hiện có. | 01/07/2026 | 01/07/2026 | Phoenix Boss, State Machine, Core System |
| 5 | - Hoàn thiện thêm hành vi và kỹ năng của Phoenix. <br> - Thiết kế lại animation flow cho Phoenix để phù hợp với các trạng thái Fly, Ground, Phase 2 và Dead. <br> - Bổ sung SFX cho các trạng thái và kỹ năng của Phoenix. <br> - Thêm Gizmo cho Phoenix để dễ chỉnh Arena, AOE, Totem và Fire Line trên nhiều map khác nhau. <br> - Điều chỉnh Fire Line Skill để rải theo vị trí Player và dừng khi chạm tường map. | 02/07/2026 | 02/07/2026 | Phoenix Animation, SFX, Gizmos |
| 6 | - Xây dựng cơ chế Battle Result cho Boss Room. <br> - Tạo hệ thống Exit Portal để Player có thể quay lại Map Lobby sau khi đánh bại Boss. <br> - Thêm cơ chế tự động đưa Player về Map Lobby khi tất cả Player chết. <br> - Tạo hệ thống Reward Table để spawn vũ khí nâng cấp sau khi Boss bị đánh bại. <br> - Sửa lỗi HealthBar Online để Client có thể thấy máu của Player giảm đúng khi bị Boss tấn công. | 03/07/2026 | 03/07/2026 | Boss Room Result, Reward System, Health Sync |
| 7 | - Sửa lỗi Battle Result trong Online để phần thưởng spawn đúng vũ khí nâng cấp thay vì spawn cùng một vũ khí mặc định. <br> - Kết nối Reward System với WeaponNetworkDatabase và NetworkWeaponPickup. <br> - Cập nhật cơ chế random 4 vũ khí thưởng từ danh sách reward. <br> - Sửa lỗi Phoenix Bullet Projectile không gây damage lên Player. <br> - Tạo thêm kỹ năng Staff Aura tăng damage cho Player đứng trong vùng. <br> - Thiết kế hướng setup vũ khí Staff vừa Heal vừa Boost Damage. | 04/07/2026 | 05/07/2026 | WeaponNetworkDatabase, NetworkWeaponPickup, Staff Aura |

### Kết quả đạt được trong tuần 11:

* Hoàn thiện được luồng Online cơ bản từ Lobby Scene đến Map Lobby và Boss Room.

* Lobby Scene đã được tối ưu lại để phục vụ cho việc test Online AWS:
  * Tạo room bằng mã.
  * Chờ Player khác tham gia.
  * Không tự động chuyển scene ngay sau khi tạo room.
  * Giữ lại các object cần thiết cho Online test.

* Xây dựng được cơ chế Revive cho Player:
  * Player không chết ngay khi hết máu.
  * Player chuyển sang trạng thái gục.
  * Thanh máu bleedout giảm dần theo thời gian.
  * Đồng đội có thể đứng gần để hồi sinh.
  * Cơ chế được thiết kế để phù hợp với Online và không ảnh hưởng đến Offline Player.

* Hoàn thành Boss Phoenix mới theo hướng Bullet Hell:
  * Fly State.
  * Ground State.
  * AOE Skill.
  * Totem Skill bắn đạn xoắn ốc.
  * Fire Line Skill.
  * Phase 2 nâng cấp kỹ năng.

* Bổ sung animation, SFX và Gizmo cho Phoenix:
  * Dễ kiểm tra vùng đánh.
  * Dễ chỉnh arena cho từng map.
  * Dễ preview AOE, Totem và Fire Line trong Scene View.

* Hoàn thiện cơ chế Boss Room Result:
  * Khi Boss bị đánh bại sẽ spawn phần thưởng.
  * Exit Portal được bật sau khi Boss chết.
  * Player có thể quay lại Map Lobby sau khi đánh Boss xong.
  * Nếu toàn bộ Player chết, hệ thống tự động đưa Player về Map Lobby.

* Hoàn thiện hệ thống reward sau Boss:
  * Spawn random 4 vũ khí từ Reward Table.
  * Hỗ trợ WeaponData nâng cấp.
  * Đồng bộ phần thưởng Online bằng NetworkWeaponPickup.
  * Kết nối với WeaponNetworkDatabase để Client và Host đều thấy đúng vũ khí.

* Sửa các lỗi Online quan trọng:
  * HealthBar của Client không cập nhật khi bị Boss tấn công.
  * Player Online không thoát được khỏi Boss Room.
  * BattleResult spawn sai vũ khí nâng cấp.
  * Phoenix Bullet Projectile không gây damage lên Player.

* Nâng cấp hệ thống vũ khí Staff:
  * Tạo Aura tăng damage gây ra cho Player đứng trong vùng.
  * Thiết kế hướng kết hợp Heal Aura và Damage Boost Aura trong cùng một kỹ năng.
  * Chuẩn bị nền tảng cho các vũ khí hỗ trợ đồng đội trong chế độ co-op.

* Tổng kết tuần:
  * Hệ thống Boss Room đã ổn định hơn cho cả Online và Offline.
  * Phoenix đã có đầy đủ bộ kỹ năng chính.
  * Reward System đã có thể dùng cho nhiều Boss khác nhau.
  * Hệ thống vũ khí bắt đầu mở rộng sang hướng support và team-based gameplay.

