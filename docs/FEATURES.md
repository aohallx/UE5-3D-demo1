# Feature List — UE5 Zombie Japan

Features inferred from the `japan1` project content tree. Update this document as systems evolve.

## Player character

- [x] Third-person character (`BP_ThirdPersonCharacter`)
- [x] Enhanced Input mapping (`IMC_Default` + input actions)
- [x] Sprint, crouch, jump, dodge roll
- [x] Vaulting over obstacles
- [x] Target lock
- [x] First-person / third-person camera toggle (`IA_PerspectiveChange` — press to switch views)
- [x] Player stats component (`BPC_PlayerStats`)
- [x] Attack system component (`BPC_AttackSystem`)
- [x] RPG character animation blueprint with locomotion blend spaces
- [x] Hit react animations (left / right)
- [x] Head look-at control rig
- [x] Lean animations while aiming

## Melee combat

- [x] Sword attack animation set (`SwordAttacks/`)
- [x] Animation notifies for sword trace loop and sphere trace
- [x] Sword camera shake (`BP_SwordCameraShake`)
- [x] Sword hit audio (`Audio/Sword_Hits`)
- [x] Assassination interface (`BPI_Assasination`)
- [x] Paired stealth kill montages (attacker + victim)
- [x] Assassination prompt UI (`WB_AssasinatePrompt`)

## Ranged combat

- [x] Pistol (`Weapon_CyberPistol`)
- [x] AK rifle (`Weapon_AK_8bit`)
- [x] Sniper rifle (`Sniper_m200`) with scope overlay (`WB_SniperScope`)
- [x] Wooden bow (`Bow1_Wood`)
- [x] Bullet actors (`BPC_Bullet`, `Bullet_Sniper`, `sm_bullet`)
- [x] Fire type enum (`E_FireType`)
- [x] Equip / unequip rifle montages
- [x] Sniper aim and lean blend spaces
- [x] Gunshot audio

## Equipment system

- [x] Equipment component (`BPC_EquipmentSystem`)
- [x] Weapon master blueprint (`Weapon_Master`, `BP_Weapon`)
- [x] Weapon data table (`DB_Weapons`)
- [x] Weapon type enums (`E_Weapon_Types`, `E_Melee_Weapons`)
- [x] Slot structs (`S_Slots`, `S_Weapons`)
- [x] Equipment menu UI (`WB_Equipment`, `WB_EquipableSlot`, `WB_ItemSlot`)
- [x] Character equipment render target preview

## Throwable / interact

- [x] Throwable object blueprint (`BP_ThrowableObject`)
- [x] Throw object animation montage
- [x] Interact input action (`IA_Interact`)

## AI — regular enemies

- [x] Generic AI pawn (`AI/AI_reg/BP_AI`)
- [x] AI controller (`BP_AIController_Generic`)
- [x] Behavior tree (`BT_AI`) + blackboard (`BD_AI`)
- [x] Tasks: patrol random point, chase target, attack target, clear investigate value
- [x] Service: distance-to-target (`BTService_GetDistanceToTarget`)
- [x] AI animation blueprint (`ABP_AI`)
- [x] Enemy spawner (`BP_EnemySpawner`)
- [x] Set-enemy-dead interface (`BPI_SetEnemyDead`)
- [x] Investigate icon UI (`WB_InvestigateIcon`)

## AI — boss

- [x] Boss AI pawn (`AI/AI_Boss/BP_AI_Boss`)
- [x] Boss controller (`BP_AIController_Boss`)
- [x] Boss behavior tree (`BT_AI_Boss`) + blackboard (`BD_AI_Boss`)
- [x] Boss health bar UI (`WB_BossHealthBar`)

## Mounts / animals

- [x] Mount interface (`BPI_Mount`)
- [x] Zebra mount blueprint (`BP_Mount_Zebra`)

## UI / HUD

- [x] Main HUD widget (`WB_HUD`)
- [x] Dummy / target health (`WB_DummyHealth`)
- [x] Boss health bar
- [x] Sniper scope overlay
- [x] Assassination prompt
- [x] Investigate icon
- [x] Custom fonts (Boogaloo, Nanum Myeongjo)

## Camera

- [x] First-person / third-person toggle (`IA_PerspectiveChange`)
- [x] Fall camera shake
- [x] Run camera shake
- [x] Sword hit camera shake

## Audio

- [x] Footsteps
- [x] Character sound attenuation (`SA_Character`)
- [x] Grunts and hit reactions
- [x] Gunshots
- [x] Sword hits
- [x] Landscape ambience
- [x] UI sounds

## VFX

- [x] Realistic Starter VFX Pack Vol2
- [x] Custom FX materials, particles, textures (`FXs/`)

## World / environment

- [x] Main level map (`ThirdPerson/Maps/Main.umap`)
- [x] Prototype / test map (`ThirdPersonMap.umap`)
- [x] Japanese shrine Megascans assets
- [x] Ultra Dynamic Sky
- [x] Landscape / landmass tooling (plugins enabled)
- [x] Megascans surface library

## Game modes

- [x] Default third-person game mode (`BP_ThirdPersonGameMode`)
- [x] Enemies game mode variant (`GM_Enemies`)

## Planned / in progress

- [ ] Additional screenshots and demo video for portfolio
- [ ] Zombie-specific enemy variants *(repo name; confirm enemy types in-editor)*
- [ ] Expanded Japan biome set
- [ ] Packaged playable demo build
