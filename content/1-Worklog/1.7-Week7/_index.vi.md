---
title: "Worklog Tuần 7"
date: 2026-06-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---


### Objective of Worklog:

* Tiếp tục hoàn thiện hệ thống combat và knockback trong project Unity.
* Khắc phục lỗi Player bị nhận knockback liên tục và không thể điều khiển trở lại.
* Xây dựng nền tảng cho Boss Minotaur bằng Finite State Machine và Core System hiện có.
* Thiết lập các trạng thái tấn công, phòng thủ, choáng, chuyển phase và tử vong của Boss.
* Kiểm tra sự đồng bộ giữa gameplay logic, Rigidbody2D, Animator và Animation Event.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Rà soát hệ thống di chuyển của Player và `TopDownKnockBackReceiver` <br><br> - Tái hiện lỗi Player bị dịch chuyển lùi liên tục sau khi nhận knockback <br><br> - Kiểm tra tương tác giữa `PlayerMove`, `Rigidbody2D` và trạng thái knockback | 01/06/2026 | 01/06/2026 | Unity Project |
| 3 | - Điều chỉnh thời gian tác dụng của knockback <br><br> - Bổ sung cơ chế kết thúc và reset trạng thái knockback <br><br> - Ngăn Player tiếp tục nhận cùng một knockback trong nhiều frame <br><br> - Khôi phục quyền điều khiển nhân vật sau khi hiệu ứng kết thúc | 02/06/2026 | 02/06/2026 | Unity Physics 2D |
| 4 | - Rà soát luồng xử lý damage và knockback giữa Enemy và Player <br><br> - Kiểm tra các interface `IDamageable` và `IKnockbackable` <br><br> - Đồng bộ Health, Poise/Stun và vận tốc của Rigidbody2D <br><br> - Kiểm thử va chạm và vùng gây sát thương của Enemy | 03/06/2026 | 03/06/2026 | Combat System |
| 5 | - Thiết lập `MinotaurBossController` <br><br> - Kết nối các component Core, Stats, Movement, Targeting và ParryReceiver <br><br> - Khởi tạo State Machine và các state cơ bản của Boss <br><br> - Bổ sung kiểm tra Stun, Death và mục tiêu Player | 04/06/2026 | 04/06/2026 | Unity C# / FSM |
| 6 | - Xây dựng luồng trạng thái tấn công cho Boss <br><br> - Thiết lập Melee, AOE, Range, Dash và Defend state <br><br> - Bổ sung logic chuyển đổi giữa Phase 1 và Phase 2 <br><br> - Thiết lập vị trí tấn công và điều kiện lựa chọn kỹ năng | 05/06/2026 | 05/06/2026 | Boss State Machine |
| 7 | - Kết nối Animator với các trạng thái của Boss <br><br> - Thiết lập các Animator bool cho Melee, AOE, Range, Dash, Defend, Stun, Phase Transition và Dead <br><br> - Kiểm tra Animation Event và quá trình kết thúc state <br><br> - Playtest, ghi nhận lỗi và tổng hợp hướng cải thiện | 06/06/2026 | 06/06/2026 | Unity Animator |


### Kết quả đạt được tuần 7:

* Khắc phục lỗi Player bị knockback liên tục và mất quyền điều khiển.
* Cải thiện luồng damage, knockback, poise và stun.
* Hoàn thiện nền tảng `MinotaurBossController`.
* Thiết lập Finite State Machine cho Boss Minotaur.
* Xây dựng các state Melee, AOE, Range, Dash và Defend.
* Bổ sung Phase Transition, Stun và Dead state.
* Kết nối các trạng thái của Boss với Animator và Animation Event.
* Hoàn thành bước playtest ban đầu và ghi nhận các lỗi cần cải thiện.


