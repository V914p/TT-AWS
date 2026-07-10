---
title: "Week 9 Worklog"
date: 2026-06-15
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---


### Objective of Worklog:

* Complete the core top-down gameplay foundation for the 2D co-op boss fight project.
* Convert legacy platformer systems into top-down systems, especially movement, aiming, combat, and weapons.
* Build the Minotaur boss mechanics with multiple states, skills, knockback, block, and parry interactions.
* Run the first multiplayer tests using Unity Netcode for GameObjects.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Analyze the current Unity project <br> - Define the direction for converting from platformer to top-down co-op boss fight <br> - Set up Player top-down movement <br> - Configure owner-based Player control in the online environment | 06/15/2026 | 06/15/2026 | Unity Documentation, Netcode for GameObjects |
| 3 | - Build the Minotaur Boss foundation <br> - Design the Boss state machine with Move, ChooseSkill, Attack, and Stun <br> - Add Boss data such as phase, movement speed, cooldown, and damage multiplier | 06/16/2026 | 06/16/2026 | Unity Documentation, Project source code |
| 4 | - Integrate the Core combat system for Boss and Player <br> - Connect Stats, Health, Poise, DamageReceiver, and KnockBackReceiver <br> - Test Boss knockback against Player <br> - Handle stun when Poise reaches zero | 06/17/2026 | 06/17/2026 | Project source code |
| 5 | - Convert the Weapon system from platformer to top-down <br> - Design a single-weapon system with left-click and right-click skills <br> - Set up Sword with normal attack, Block, and Parry <br> - Fix Block/Parry direction based on top-down aim | 06/18/2026 | 06/18/2026 | Unity Documentation, Project source code |
| 6 | - Debug Block and Parry mechanics <br> - Fix null reference errors related to TopDownAim, DamageReceiver, and KnockBackReceiver <br> - Test Block/Parry windows using animation events <br> - Prevent Player from receiving continuous knockback when hit | 06/19/2026 | 06/19/2026 | Project source code |
| 7 | - Complete initial weapon tests for Sword, Bow, and Staff <br> - Test left-click and right-click input <br> - Tune animation events for AttackAction, EnterAttackPhase, and AnimationFinished | 06/20/2026 | 06/20/2026 | Unity Documentation, Project source code |
| Sunday | - Run integrated offline and local online gameplay testing <br> - Check Player movement, aim direction, animation sync, and combat interaction <br> - Record issues to be handled next week | 06/21/2026 | 06/21/2026 | Netcode for GameObjects, Project source code |

### Week 9 Achievements:

* Completed the foundation of top-down Player movement.
* Player can move in four directions using Rigidbody2D.
* Player can aim based on mouse position.
* Movement direction and look direction are synchronized in the online environment.
* Only the Player owner can control their own character.
* Built the Minotaur Boss with a basic state machine:
  * Move.
  * ChooseSkill.
  * Attack.
  * Stun.
  * Phase transition.
* Implemented the foundation for two Boss phases and multiple skills:
  * Melee Attack.
  * AOE Attack.
  * Range Attack.
  * Dash Attack.
  * Defend.
* Integrated Boss with the Core combat system.
* Converted the first part of the Weapon system into top-down gameplay.
* Fixed important issues related to continuous knockback, Block/Parry direction, animation events, and null references.
* Completed the first round of offline and local multiplayer testing with Unity Netcode.


