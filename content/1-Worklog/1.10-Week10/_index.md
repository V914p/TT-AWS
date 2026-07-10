---
title: "Week 10 Worklog"
date: 2026-06-22
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Objective of Worklog:

* Complete the top-down weapon system with multiple weapon types.
* Add visual effects for attacks, Block, Parry, and projectiles.
* Create debug tools to visualize hitboxes, Block direction, and Parry direction.
* Complete Unity-side online testing.
* Prepare the first AWS deployment workflow for building and hosting the game server.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Complete the Lobby and Map Lobby flow <br> - Design the Boss Room entry flow <br> - Test online/offline Player spawning <br> - Prepare the BossRoom_Minotaur scene | 06/22/2026 | 06/22/2026 | Unity Documentation, Netcode for GameObjects |
| 3 | - Set up Cinemachine camera for top-down gameplay <br> - Configure the camera to follow the local Player <br> - Set up CameraBounds and fix the issue where Player is pushed outside the map <br> - Test camera behavior in offline and online modes | 06/23/2026 | 06/23/2026 | Unity Cinemachine Documentation |
| 4 | - Complete gameplay UI system <br> - Link Stats with Health, Mana, and Poise UI <br> - Test Weapon Pickup offline/online <br> - Fix weapon pickup issues and incorrect WeaponData assignment | 06/24/2026 | 06/24/2026 | Unity Documentation, Project source code |
| 5 | - Optimize NetworkPlayer and PlayerMove <br> - Test multiple clients in the same LobbyScene <br> - Fix NetworkManager and UnityTransport issues <br> - Test online movement, aim, weapon switching, and map entry | 06/25/2026 | 06/25/2026 | Netcode for GameObjects |
| 6 | - Complete multiple weapons: Sword, Spear, Bow, and Staff <br> - Set up Spear with two left-click combo attacks and quick right-click Parry <br> - Set up Bow Rapid Fire/Burst Rapid Fire <br> - Set up Staff homing magic bolt and heal aura <br> - Add left-click and right-click skill icons to WeaponData | 06/26/2026 | 06/26/2026 | Unity Documentation, Project source code |
| 7 | - Design Slash Effect Prefab system for weapons <br> - Set up Shield Wave effect when Block is pressed <br> - Set up Hold Pulse effect while holding Block <br> - Set up Spark effect only when Block or Parry succeeds <br> - Add projectile trail for Arrow and Magic Bolt | 06/27/2026 | 06/27/2026 | Unity Documentation, Project source code |
| Sunday | - Create hitbox debug tools for ActionHitBox <br> - Draw Block and Parry direction previews in Scene View <br> - Tune attack areas for Sword, Spear, and Shield <br> - Prepare AWS architecture with EC2, Lambda Function URL, and DynamoDB <br> - Start preparing Linux Dedicated Server build and EC2 SSH connection | 06/28/2026 | 06/28/2026 | AWS Documentation, Unity Dedicated Server Documentation |

### Week 10 Achievements:

* Completed the top-down weapon system with multiple weapon types:
  * Sword supports combo attacks, Block, and Parry.
  * Spear supports two left-click combo attacks and quick right-click Parry without holding Block.
  * Bow supports Rapid Fire and Burst Rapid Fire.
  * Staff supports homing magic bolt and healing/buff skill.
* Added skill icon support to WeaponData:
  * Left-click skill icon.
  * Right-click skill icon.
  * Primary skill name.
  * Secondary skill name.
  * Ready to display on gameplay UI.
* Improved combat visual feedback:
  * Slash Effect Prefab for Sword.
  * Stab Effect Prefab for Spear.
  * Wave Effect for Shield when Block is pressed.
  * Hold Pulse Effect while holding Block.
  * Spark Effect only when Block or Parry succeeds.
  * Trail effect for Arrow and Magic projectile.
* Created debug tools for combat tuning:
  * Display ActionHitBox based on aim direction.
  * Display the real hitbox when animation calls AttackAction.
  * Display Block Direction.
  * Display Parry Direction.
  * Make attack range and hitbox tuning more visual in Scene View.
* Completed Unity-side online testing:
  * Host and Client can enter the Lobby.
  * Online Player movement and aiming work correctly.
  * Weapons work in the online environment.
  * Boss Room and Map Lobby are ready for further online testing.
* Prepared the first AWS deployment plan:
  * Selected the 3-service model: EC2, Lambda Function URL, and DynamoDB.
  * Prepared the Unity Linux Dedicated Server direction.
  * Planned the server build upload process to EC2.
  * Fixed the PEM file permission issue when connecting to EC2 from Windows.
* Week 10 summary: offline and online gameplay became stable, weapon systems and visual feedback were improved, and the project is ready to move into server build and external online testing.


