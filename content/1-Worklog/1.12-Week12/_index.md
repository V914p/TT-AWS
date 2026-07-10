---

title: "Week 12 Worklog"
date: 2026-07-06
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
-----------------------


### Objective of Worklog:

* Finalize the Unity-side online gameplay testing before moving to external online deployment.
* Prepare the AWS deployment workflow for the RoughLife multiplayer game server.
* Build and configure the Unity Linux Dedicated Server for cloud hosting.
* Set up the first AWS architecture direction using EC2, Lambda Function URL, and DynamoDB.
* Organize project documentation, worklogs, and event reports for final submission.

### Tasks to be carried out this week:

| Day       | Task                                                                                                                                                                                                                                                                                                                                                                    | Start Date | Completion Date | Reference Material                                      |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ------------------------------------------------------- |
| Monday    | - Review the completed Unity online gameplay flow <br> - Verify Lobby, Map Lobby, Boss Room, Player movement, aiming, and weapon interaction <br> - Confirm that the online system is ready for external server testing                                                                                                                                                 | 07/06/2026 | 07/06/2026      | Unity Documentation, Netcode for GameObjects            |
| Tuesday   | - Finalize combat debugging tools <br> - Check ActionHitBox preview, Block Direction preview, and Parry Direction preview <br> - Tune weapon hitboxes for Sword, Spear, Shield, Bow, and Staff <br> - Confirm that weapon mechanics work correctly in offline and online modes                                                                                          | 07/07/2026 | 07/07/2026      | Unity Documentation, Project source code                |
| Wednesday | - Plan the AWS deployment architecture for RoughLife <br> - Select the initial 3-service model: EC2, Lambda Function URL, and DynamoDB <br> - Define the online flow: Client requests room code, receives server IP/port, and connects to the dedicated server <br> - Review optional services such as S3, CloudFront, CloudWatch, and GameLift for future improvements | 07/08/2026 | 07/08/2026      | AWS Documentation, Unity Dedicated Server Documentation |
| Thursday  | - Prepare Unity Linux Dedicated Server build <br> - Create or review ServerBoot and server bootstrap logic <br> - Configure UnityTransport for UDP connection <br> - Prepare Windows Client build for external player testing <br> - Start configuring EC2 server, Security Group, SSH access, and UDP port 7777                                                        | 07/09/2026 | 07/09/2026      | Unity Dedicated Server, AWS EC2 Documentation           |
| Friday    | - Upload and test the dedicated server build workflow on AWS EC2 <br> - Fix Windows PEM private key permission issue when using SSH/SCP <br> - Continue preparing Lambda Function URL and DynamoDB room table design <br> - Reformat and translate weekly worklogs and event reports for documentation consistency                                                      | 07/10/2026 | 07/10/2026      | AWS EC2, AWS Lambda, DynamoDB, Project Documentation    |

### Week 12 Achievements:

* Completed the Unity-side online gameplay validation:

  * Host and Client can join the online flow.
  * Online Player movement and aiming work correctly.
  * Weapons can be used in the online environment.
  * Map Lobby and Boss Room flow are ready for external testing.

* Finalized combat and weapon tuning tools:

  * ActionHitBox can be visualized clearly.
  * Block Direction can be previewed in Scene View.
  * Parry Direction can be previewed in Scene View.
  * Weapon hitboxes are easier to adjust for different attack ranges and weapon types.

* Prepared the first AWS deployment model for RoughLife:

  * EC2 is used to host the Unity Dedicated Server.
  * Lambda Function URL is planned as the Room API.
  * DynamoDB is planned to store temporary room information.
  * The client can receive server address and port before connecting to the game server.

* Prepared the Unity Dedicated Server deployment workflow:

  * Linux Dedicated Server build direction was defined.
  * Windows Client build direction was prepared.
  * UnityTransport UDP connection was reviewed.
  * Server startup flow and port configuration were planned.

* Started AWS EC2 server setup:

  * Created or prepared the EC2 server environment.
  * Reviewed Security Group requirements.
  * Planned UDP port 7777 for game traffic.
  * Used SSH/SCP workflow to upload and manage server files.

* Fixed an important AWS connection issue:

  * Identified that the PEM private key file had unsafe permissions on Windows.
  * Adjusted file permission using Windows permission commands.
  * Prepared the SSH/SCP workflow for uploading the Linux server build.

* Improved project documentation:

  * Reformatted Vietnamese worklog files to match the required report template.
  * Created English worklog versions based on the Vietnamese reports.
  * Revised event report content while keeping the original layout.
  * Prepared documentation for project submission and GitHub presentation.

* Week 12 summary: Unity online testing was completed successfully, the weapon and combat debugging tools became stable, and the project moved into the AWS deployment preparation phase. The team is now ready to continue testing RoughLife with external players through a cloud-hosted dedicated server.

