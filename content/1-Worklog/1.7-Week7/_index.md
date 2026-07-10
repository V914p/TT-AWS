---
title: "Week 7 Worklog"
date: 2026-06-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---


### Objective of Worklog:

* Continue improving the combat and knockback systems in the Unity project.
* Fix the issue where Player receives continuous knockback and cannot regain control.
* Build the foundation for the Minotaur Boss using the existing FSM and Core System.
* Set up Boss attack, defense, stun, phase transition, and death states.
* Test synchronization between gameplay logic, Rigidbody2D, Animator, and Animation Events.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Review Player movement and TopDownKnockBackReceiver <br> - Reproduce the issue where Player is continuously pushed back after receiving knockback <br> - Check interaction between PlayerMove, Rigidbody2D, and knockback state | 06/01/2026 | 06/01/2026 | Unity Project |
| 3 | - Adjust knockback duration <br> - Add logic to end and reset knockback state <br> - Prevent Player from receiving the same knockback across multiple frames <br> - Restore character control after knockback ends | 06/02/2026 | 06/02/2026 | Unity Physics 2D |
| 4 | - Review damage and knockback flow between Enemy and Player <br> - Check IDamageable and IKnockbackable interfaces <br> - Synchronize Health, Poise/Stun, and Rigidbody2D velocity <br> - Test collision and Enemy damage areas | 06/03/2026 | 06/03/2026 | Combat System |
| 5 | - Set up MinotaurBossController <br> - Connect Core, Stats, Movement, Targeting, and ParryReceiver components <br> - Initialize State Machine and basic Boss states <br> - Add Stun, Death, and Player target checking | 06/04/2026 | 06/04/2026 | Unity C# / FSM |
| 6 | - Build Boss attack state flow <br> - Set up Melee, AOE, Range, Dash, and Defend states <br> - Add Phase 1 and Phase 2 transition logic <br> - Set up attack positions and skill selection conditions | 06/05/2026 | 06/05/2026 | Boss State Machine |
| 7 | - Connect Animator with Boss states <br> - Set Animator bools for Melee, AOE, Range, Dash, Defend, Stun, Phase Transition, and Dead <br> - Check Animation Events and state finish flow <br> - Playtest and summarize issues for improvement | 06/06/2026 | 06/06/2026 | Unity Animator |

### Week 7 Achievements:

* Fixed the continuous knockback issue.
* Player can regain control after knockback ends.
* Improved the interaction between input, Rigidbody2D movement, and knockback state.
* Stabilized the Combat System for damage, knockback, and stun handling.
* Created the foundation of the Minotaur Boss architecture.
* Set up the main Boss states:
  * Melee Attack.
  * AOE Attack.
  * Range Attack.
  * Dash Attack.
  * Defend.
  * Stun.
  * Phase Transition.
  * Dead.
* Connected Boss gameplay logic with Animator and Animation Events.
* Identified areas that need further tuning, such as damage timing, state transition, and skill cooldown.


