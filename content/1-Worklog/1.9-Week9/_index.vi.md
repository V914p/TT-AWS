---
title: "Worklog Tuần 9"
date: 2026-06-15
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---


### Objective of Worklog:

* :
* Hoàn thiện nền tảng gameplay top-down cho dự án game 2D co-op boss fight.
* Chuyển đổi các hệ thống cũ từ platformer sang top-down, đặc biệt là di chuyển, aim, combat và weapon.
* Xây dựng cơ chế boss Minotaur gồm nhiều trạng thái, nhiều kỹ năng và có thể tương tác với hệ thống knockback, block, parry.
* Kiểm thử bước đầu cơ chế multiplayer bằng Unity Netcode for GameObjects.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Phân tích lại project Unity hiện tại<br> - Xác định hướng chuyển game từ platformer sang top-down co-op boss fight<br> - Thiết lập lại Player top-down movement<br> - Cấu hình điều khiển Player theo owner trong môi trường online | 15/06/2026 | 15/06/2026 | Unity Documentation, Netcode for GameObjects |
| 3 | - Xây dựng nền tảng Boss Minotaur<br> - Thiết kế state machine cho Boss gồm Move, ChooseSkill, Attack và Stun<br> - Bổ sung dữ liệu Boss gồm phase, tốc độ di chuyển, cooldown và damage multiplier | 16/06/2026 | 16/06/2026 | Unity Documentation, Project source code |
| 4 | - Tích hợp hệ thống Core combat cho Boss và Player<br> - Kết nối Stats, Health, Poise, DamageReceiver và KnockBackReceiver<br> - Kiểm thử Boss gây knockback lên Player<br> - Xử lý cơ chế stun khi poise giảm về 0 | 17/06/2026 | 17/06/2026 | Project source code |
| 5 | - Chuyển đổi hệ thống Weapon từ platformer sang top-down<br> - Thiết kế hướng dùng một vũ khí chính với hai kỹ năng chuột trái và chuột phải<br> - Setup Sword với đòn đánh thường, Block và Parry<br> - Sửa lỗi Block/Parry theo hướng aim top-down | 18/06/2026 | 18/06/2026 | Unity Documentation, Project source code |
| 6 | - Debug cơ chế Block và Parry<br> - Sửa lỗi null reference khi dùng TopDownAim, DamageReceiver và KnockBackReceiver<br> - Kiểm thử cửa sổ Block/Parry bằng animation event<br> - Đảm bảo Player không bị knockback liên tục khi nhận hit | 19/06/2026 | 19/06/2026 | Project source code |
| 7 | - Hoàn thiện bước đầu các loại vũ khí test như Sword, Bow và Staff<br> - Kiểm thử input chuột trái/chuột phải<br> - Tinh chỉnh animation event cho AttackAction, EnterAttackPhase và AnimationFinished | 20/06/2026 | 20/06/2026 | Unity Documentation, Project source code |
| CN | - Kiểm thử tổng hợp gameplay offline và online local<br> - Kiểm tra Player movement, aim direction, animation sync và combat interaction<br> - Ghi nhận các lỗi cần xử lý tiếp trong tuần sau | 21/06/2026 | 21/06/2026 | Netcode for GameObjects, Project source code |


### Kết quả đạt được tuần 9:

* Hoàn thiện nền tảng Player top-down movement, bao gồm:
* Di chuyển 4 hướng bằng Rigidbody2D.
* Aim theo vị trí chuột.
* Đồng bộ hướng di chuyển và hướng nhìn trong môi trường online.
* Chỉ Player owner mới được điều khiển nhân vật của mình.
* Xây dựng được Boss Minotaur với state machine cơ bản:
* Move.
* ChooseSkill.
* Attack.
* Stun.
* Phase transition.
* Boss Minotaur đã có nền tảng 2 phase và nhiều loại kỹ năng:
* Melee Attack.
* AOE Attack.
* Range Attack.
* Dash Attack.
* Defend.
* Tích hợp Boss với hệ thống Core combat:
* Health.
* Poise.
* DamageReceiver.
* KnockBackReceiver.
* ParryReceiver.
* Death handling.
* Chuyển đổi thành công bước đầu hệ thống Weapon sang top-down:
* Vũ khí dùng chuột trái cho kỹ năng chính.
* Vũ khí dùng chuột phải cho kỹ năng phụ.
* Sword có thể đánh thường, Block và Parry.
* Sửa được nhiều lỗi quan trọng:
* Player bị knockback liên tục.
* Block/Parry không nhận đúng hướng top-down.
* Animation event không kích hoạt đúng phase.
* Một số lỗi null reference trong Core combat.
* Hoàn thành bước thử nghiệm đầu tiên cho gameplay offline và multiplayer local bằng Unity Netcode.


