---
title: "Week 11 Worklog"
date: 2026-07-05
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Objective of Worklog:

* Complete important Online features for the TopDown co-op boss fight game.
* Integrate the room creation, room joining, and scene transition flow between Lobby Scene, Map Lobby, and Boss Room.
* Develop a new Bullet Hell style Phoenix Boss with multiple states and skills.
* Complete the Boss Room result system, including returning to Map Lobby, checking if all players are dead, and spawning rewards after defeating the Boss.
* Improve the weapon, reward, and support skill systems for the Player.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Continued improving the Online flow for the game. <br> - Checked the Lobby Scene so players can create rooms, enter room codes, and prepare to enter Map Lobby. <br> - Cleaned up unnecessary test objects in Lobby Scene and kept only the required objects for AWS Online testing. <br> - Adjusted the Online flow so creating a room does not immediately move the player to Map Lobby, allowing other players to join first. | 06/29/2026 | 06/29/2026 | Unity Netcode, AWS Room API |
| 3 | - Re-analyzed the Core System to design a Player Revive mechanism. <br> - Designed the downed state, bleedout health timer, and teammate revive interaction. <br> - Ensured that the Revive system can be used for Online gameplay without affecting the Offline Player. <br> - Checked the Player death flow inside Boss Rooms. | 06/30/2026 | 06/30/2026 | Core System, Stats, Revive System |
| 4 | - Started developing a new Phoenix Boss for the game. <br> - Designed Phoenix as a Bullet Hell boss with Fly State, Ground State, AOE Skill, Totem Skill, Fire Line Skill, and Phase 2. <br> - Created supporting prefabs such as Phoenix Bullet Totem, Phoenix Bullet Projectile, and Phoenix Fire Line Hazard. <br> - Fixed issues that occurred when integrating Phoenix with the existing State Machine and Core System. | 07/01/2026 | 07/01/2026 | Phoenix Boss, State Machine, Core System |
| 5 | - Improved Phoenix behavior and skill flow. <br> - Reworked the Phoenix animation flow to match Fly, Ground, Phase 2, and Dead states. <br> - Added SFX for Phoenix states and skills. <br> - Added Gizmos for Phoenix to make Arena, AOE, Totem, and Fire Line setup easier across different maps. <br> - Adjusted Fire Line Skill so it targets player positions and stops when reaching map walls. | 07/02/2026 | 07/02/2026 | Phoenix Animation, SFX, Gizmos |
| 6 | - Developed the Boss Room Battle Result system. <br> - Created an Exit Portal system so players can return to Map Lobby after defeating the Boss. <br> - Added an automatic return-to-lobby flow when all players are dead. <br> - Created a Reward Table system to spawn upgraded weapons after the Boss is defeated. <br> - Fixed the Online HealthBar issue so Client players can correctly see health reduction when hit by the Boss. | 07/03/2026 | 07/03/2026 | Boss Room Result, Reward System, Health Sync |
| 7 | - Fixed the Online Battle Result reward issue so upgraded weapons spawn correctly instead of spawning the same default weapon. <br> - Connected the Reward System with WeaponNetworkDatabase and NetworkWeaponPickup. <br> - Updated the reward system to randomly spawn 4 weapons from the reward list. <br> - Fixed Phoenix Bullet Projectile not dealing damage to the Player. <br> - Created a Staff Aura skill that increases outgoing damage for players standing inside the aura. <br> - Designed the setup direction for a Staff weapon that can both Heal and Boost Damage. | 07/04/2026 | 07/05/2026 | WeaponNetworkDatabase, NetworkWeaponPickup, Staff Aura |

### Week 11 Achievements:

* Completed the basic Online flow from Lobby Scene to Map Lobby and Boss Room.

* Optimized the Lobby Scene for AWS Online testing:
  * Create room by code.
  * Wait for other players to join.
  * Prevent automatic scene transition immediately after room creation.
  * Keep only the necessary objects for Online testing.

* Designed and implemented the Player Revive system:
  * Players do not die immediately when their health reaches zero.
  * Players enter a downed state.
  * Bleedout health decreases over time.
  * Teammates can stand nearby to revive downed players.
  * The system is designed for Online gameplay while keeping Offline gameplay unaffected.

* Completed the new Bullet Hell style Phoenix Boss:
  * Fly State.
  * Ground State.
  * AOE Skill.
  * Spiral projectile Totem Skill.
  * Fire Line Skill.
  * Phase 2 skill upgrades.

* Added animation, SFX, and Gizmos for Phoenix:
  * Easier to check attack areas.
  * Easier to configure arenas for different maps.
  * Easier to preview AOE, Totem, and Fire Line behavior in Scene View.

* Completed the Boss Room Result system:
  * Rewards spawn after the Boss is defeated.
  * Exit Portal is activated after the Boss dies.
  * Players can return to Map Lobby after finishing a Boss fight.
  * If all players die, the system automatically returns them to Map Lobby.

* Completed the Boss reward system:
  * Randomly spawns 4 weapons from the Reward Table.
  * Supports upgraded WeaponData.
  * Synchronizes reward pickups Online using NetworkWeaponPickup.
  * Connects with WeaponNetworkDatabase so both Host and Client see the correct weapon.

* Fixed important Online issues:
  * Client HealthBar did not update when hit by the Boss.
  * Online players could not exit the Boss Room.
  * BattleResult spawned incorrect upgraded weapons.
  * Phoenix Bullet Projectile did not deal damage to players.

* Improved the Staff weapon system:
  * Created a Damage Boost Aura for players standing inside the aura.
  * Designed a combined Heal Aura and Damage Boost Aura skill.
  * Prepared the foundation for more co-op support weapons.

* Weekly summary:
  * The Boss Room system is now more stable for both Online and Offline gameplay.
  * Phoenix now has a complete main skill set.
  * The Reward System can be reused for multiple Bosses.
  * The weapon system is expanding toward support and team-based gameplay.

