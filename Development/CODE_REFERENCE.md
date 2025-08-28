# Code Reference & File Structure Guide

## Overview
This document provides a comprehensive reference for all code files, assets, and their specific purposes within the Tactical Team Shooter project. Each file is organized by system and includes detailed descriptions of functionality and dependencies.

## Scripts Directory Structure

### Core System Files (`Scripts/Core/`)

#### GameManager.java
**Purpose**: Central game state management and coordination
**Functionality**:
- Game initialization and shutdown
- Scene management and transitions
- Global game state tracking
- System coordination and communication
- Main game loop control

#### InputManager.java
**Purpose**: Centralized input handling and processing
**Functionality**:
- Keyboard and mouse input processing
- Input mapping and configuration
- Action binding system
- Input validation and filtering
- Control scheme management

#### ConfigManager.java
**Purpose**: Configuration and settings management
**Functionality**:
- Load/save game settings
- Graphics options management
- Audio settings control
- Key binding configuration
- Performance settings

#### SceneManager.java
**Purpose**: Scene loading, unloading, and transition management
**Functionality**:
- Scene lifecycle management
- Smooth scene transitions
- Resource cleanup between scenes
- Scene state persistence
- Loading screen management

#### ResourceManager.java
**Purpose**: Asset loading, caching, and memory management
**Functionality**:
- Texture loading and caching
- Audio file management
- Font and UI asset handling
- Memory-efficient asset disposal
- Batch loading operations

### Combat System Files (`Scripts/Combat/`)

#### CombatManager.java
**Purpose**: Core combat system coordination
**Functionality**:
- Combat state management
- Damage calculation and application
- Team-based combat rules
- Combat event coordination
- Victory condition checking

#### WeaponSystem.java
**Purpose**: Weapon mechanics and management
**Functionality**:
- Weapon switching and selection
- Ammunition tracking
- Weapon upgrade system
- Recoil pattern management
- Weapon attachment handling

#### Weapon.java (Base Class)
**Purpose**: Abstract base class for all weapons
**Properties**:
- Damage, fire rate, range statistics
- Ammunition capacity and reload time
- Recoil patterns and accuracy modifiers
- Sound and visual effect references
- Upgrade compatibility flags

#### AssaultRifle.java
**Purpose**: Assault rifle weapon implementation
**Specifications**:
- AK-47 Style: 35 damage, 600 RPM, 30 rounds
- M4 Style: 30 damage, 750 RPM, 30 rounds
- High/medium recoil patterns
- Long-range effectiveness

#### SubmachineGun.java
**Purpose**: SMG weapon implementation
**Specifications**:
- MP5 Style: 25 damage, 900 RPM, 30 rounds
- High fire rate, low damage
- Medium range effectiveness
- High mobility bonus

#### Shotgun.java
**Purpose**: Shotgun weapon implementation
**Specifications**:
- 120 damage (close range), 60 RPM, 8 shells
- Spread pattern calculation
- Distance-based damage falloff
- Short-range specialization

#### SniperRifle.java
**Purpose**: Sniper rifle weapon implementation
**Specifications**:
- 120 damage, 40 RPM, 5 rounds
- Scope zoom functionality (2x)
- Very long range capability
- High accuracy, low mobility

#### Pistol.java
**Purpose**: Pistol weapon implementation
**Specifications**:
- 40 damage, 300 RPM, 12 rounds
- High accuracy, medium range
- Backup weapon functionality
- Fast draw and reload

#### HealthSystem.java
**Purpose**: Player health and damage management
**Functionality**:
- Health tracking (150 HP base)
- Damage application and mitigation
- Death and respawn handling
- Health regeneration (if applicable)
- Damage history tracking

#### ArmorSystem.java
**Purpose**: Armor mechanics and protection
**Functionality**:
- Light Armor: +25 HP, -10% speed
- Heavy Armor: +50 HP, -20% speed
- Armor degradation over time
- Pickup and equip mechanics
- Visual armor indicators

#### DefenseSystem.java
**Purpose**: Defensive mechanics implementation
**Functionality**:
- Cover detection and protection
- Dodge roll mechanics (3s cooldown, 0.2s invincibility)
- Crouching system (accuracy bonus, smaller hitbox)
- Leaning around corners
- Defensive positioning bonuses

#### MeleeSystem.java
**Purpose**: Melee combat mechanics
**Functionality**:
- Hand-to-hand combat (punch, kick, grapple)
- Melee weapon handling (knife, bat, sword)
- Range detection and hit registration
- Combo system implementation
- Melee vs ranged balance

### Networking System Files (`Scripts/Networking/`)

#### NetworkManager.java
**Purpose**: Core networking system management
**Functionality**:
- Client-server connection handling
- Network protocol implementation
- Connection quality monitoring
- Reconnection and error recovery
- Network security measures

#### PlayerSync.java
**Purpose**: Player state synchronization
**Functionality**:
- Position and rotation sync
- Animation state sync
- Team assignment sync
- Player identification
- Lag compensation

#### CombatSync.java
**Purpose**: Combat system networking
**Functionality**:
- Hit detection synchronization
- Weapon firing sync
- Damage application sync
- Kill confirmation
- Combat effect sync

#### GameStateSync.java
**Purpose**: Game state networking
**Functionality**:
- Match state synchronization
- Score and timer sync
- Objective state sync
- Victory condition sync
- Round management sync

#### MatchmakingSystem.java
**Purpose**: Player matching and lobby management
**Functionality**:
- Skill-based matchmaking
- Queue management
- Party/group support
- Server selection
- Match balancing

### User Interface Files (`Scripts/UI/`)

#### UIManager.java
**Purpose**: UI system coordination and management
**Functionality**:
- UI element lifecycle management
- Screen transition handling
- Input routing to UI elements
- UI state persistence
- Dynamic UI scaling

#### MainMenuUI.java
**Purpose**: Main menu interface implementation
**Functionality**:
- Menu navigation system
- Settings integration
- Play mode selection
- Profile management
- News and updates display

#### HUDManager.java
**Purpose**: In-game HUD management
**Functionality**:
- Health/armor bar updates
- Ammo counter display
- Crosshair management
- Minimap integration
- Kill feed display

#### ScoreboardUI.java
**Purpose**: Match scoreboard implementation
**Functionality**:
- Player statistics display
- Team score tracking
- Real-time stat updates
- End-game statistics
- Performance metrics

#### SettingsUI.java
**Purpose**: Settings and configuration interface
**Functionality**:
- Graphics settings controls
- Audio level adjustments
- Key binding interface
- Performance options
- Save/load configurations

### AI System Files (`Scripts/AI/`)

#### AIController.java
**Purpose**: AI bot behavior control
**Functionality**:
- Decision making system
- Behavior state management
- Team coordination
- Difficulty scaling
- Performance optimization

#### AIMovement.java
**Purpose**: AI pathfinding and movement
**Functionality**:
- Pathfinding algorithm
- Obstacle avoidance
- Formation movement
- Cover seeking behavior
- Movement prediction

#### AICombat.java
**Purpose**: AI combat behavior
**Functionality**:
- Target selection and prioritization
- Weapon choice logic
- Shooting accuracy scaling
- Combat tactics implementation
- Team coordination

#### AIObjective.java
**Purpose**: AI objective understanding
**Functionality**:
- Game mode comprehension
- Objective prioritization
- Team role assignment
- Strategic positioning
- Adaptive behavior

### Utility Files (`Scripts/Utils/`)

#### MathUtils.java
**Purpose**: Mathematical calculations and utilities
**Functionality**:
- Vector calculations
- Distance and angle computations
- Collision detection helpers
- Random number generation
- Performance optimized math

#### AudioUtils.java
**Purpose**: Audio system utilities
**Functionality**:
- 3D audio positioning
- Volume calculation helpers
- Audio file format handling
- Sound mixing utilities
- Audio performance optimization

#### FileUtils.java
**Purpose**: File I/O operations and utilities
**Functionality**:
- Save/load game data
- Configuration file handling
- Asset file management
- Error handling for file ops
- Cross-platform compatibility

## Assets Directory Structure

### Character Assets (`Assets/Characters/`)

#### PlayerCharacter.png
**Purpose**: Base player character sprite
**Specifications**:
- 32x32 pixel sprite
- Team color variations (Red/Blue)
- Multiple animation frames
- Optimized for top-down view

#### CharacterAnimations/
**Purpose**: Character animation sprite sheets
**Contents**:
- Walking animation (8 frames)
- Running animation (8 frames)
- Idle animation (4 frames)
- Combat animations (various)

#### CharacterCustomization/
**Purpose**: Character customization assets
**Contents**:
- Hat variations (cap, beanie, helmet, etc.)
- Backpack options (tactical, school, hiking)
- Accessory items (glasses, goggles)
- Unlockable skins (camo, elite, golden)

### Weapon Assets (`Assets/Weapons/`)

#### WeaponSprites/
**Purpose**: Individual weapon visual assets
**Contents**:
- AssaultRifle_AK47.png (32x16 pixels)
- AssaultRifle_M4.png (32x16 pixels)
- SMG_MP5.png (28x12 pixels)
- Shotgun_Pump.png (36x14 pixels)
- Sniper_BoltAction.png (48x12 pixels)
- Pistol_Standard.png (20x12 pixels)

#### MeleeWeapons/
**Purpose**: Melee weapon visual assets
**Contents**:
- Knife.png (16x4 pixels)
- BaseballBat.png (32x8 pixels)
- Sword.png (40x8 pixels)
- Fist icons for hand-to-hand combat

#### WeaponEffects/
**Purpose**: Weapon visual effects
**Contents**:
- Muzzle flash sprites
- Shell ejection animations
- Bullet impact effects
- Reload visual indicators

### Map Assets (`Assets/Maps/`)

#### FactoryFloor/
**Purpose**: Factory map visual elements
**Contents**:
- FactoryTiles.png (tile set)
- ConveyorBelt.png (animated)
- Machinery.png (cover objects)
- IndustrialLighting.png
- FactoryBackground.png

#### UrbanStreets/
**Purpose**: Urban map visual elements
**Contents**:
- StreetTiles.png (asphalt, sidewalk)
- Buildings.png (multi-story facades)
- Vehicles.png (cars, trucks for cover)
- StreetFurniture.png (signs, lights)
- UrbanBackground.png

#### MilitaryBase/
**Purpose**: Military map visual elements
**Contents**:
- BaseTiles.png (concrete, dirt)
- Bunkers.png (military structures)
- Watchtowers.png (elevated positions)
- MilitaryVehicles.png
- MilitaryBackground.png

### UI Assets (`Assets/UI/`)

#### HUD/
**Purpose**: In-game interface elements
**Contents**:
- HealthBar.png (health indicator)
- AmmoCounter.png (ammunition display)
- Crosshair.png (aiming reticle)
- Minimap.png (map display)
- ScoreDisplay.png (score indicators)

#### Menus/
**Purpose**: Menu interface elements
**Contents**:
- MainMenuBackground.png
- ButtonStyles.png (normal, hover, pressed)
- SettingsIcons.png (audio, video, controls)
- LoadingScreen.png
- VictoryDefeatScreens.png

#### Icons/
**Purpose**: Various game icons
**Contents**:
- WeaponIcons.png (weapon selection)
- ItemIcons.png (grenades, medkits)
- TeamIcons.png (red/blue indicators)
- ObjectiveIcons.png (capture points, etc.)

### Effect Assets (`Assets/Effects/`)

#### Particles/
**Purpose**: Particle effect textures
**Contents**:
- ExplosionParticles.png
- SmokeParticles.png
- BloodSplatters.png
- HitSparks.png
- MuzzleFlash.png

#### Lighting/
**Purpose**: Lighting and shadow effects
**Contents**:
- CharacterShadow.png
- DynamicLighting.png
- MapLighting.png
- EnvironmentalEffects.png

## Scenes Directory Structure

### MainMenu (`Scenes/MainMenu/`)

#### MainMenu.scene
**Purpose**: Primary menu scene
**Contents**:
- Menu UI layout
- Background elements
- Navigation logic
- Settings integration

### GameModes (`Scenes/GameModes/`)

#### TeamDeathmatch.scene
**Purpose**: Team Deathmatch game mode scene
**Contents**:
- Match timer setup
- Kill counter logic
- Respawn system
- Score tracking

#### CaptureAndHold.scene
**Purpose**: Capture and Hold game mode scene
**Contents**:
- Control point setup
- Capture progress tracking
- Territory control logic
- Score accumulation

#### SearchAndDestroy.scene
**Purpose**: Search and Destroy game mode scene
**Contents**:
- Bomb site locations
- Round-based logic
- Elimination tracking
- Bomb mechanics

#### KingOfTheHill.scene
**Purpose**: King of the Hill game mode scene
**Contents**:
- Central control point
- Control time tracking
- Hill contest mechanics
- Victory conditions

#### EscortMission.scene
**Purpose**: Escort Mission game mode scene
**Contents**:
- Payload object setup
- Movement mechanics
- Checkpoint system
- Team role assignment

### Maps (`Scenes/Maps/`)

#### FactoryFloorMap.scene
**Purpose**: Factory Floor map implementation
**Contents**:
- Map layout and collision
- Spawn point configuration
- Environmental elements
- Lighting setup

#### UrbanStreetsMap.scene
**Purpose**: Urban Streets map implementation
**Contents**:
- Building layouts
- Vehicle placement
- Multi-level design
- Street lighting

#### MilitaryBaseMap.scene
**Purpose**: Military Base map implementation
**Contents**:
- Base layout design
- Bunker systems
- Watchtower positions
- Tactical elements

## File Dependencies and Relationships

### Core System Dependencies
```
GameManager -> SceneManager, InputManager, ConfigManager
SceneManager -> ResourceManager
InputManager -> ConfigManager
ResourceManager -> All Asset files
```

### Combat System Dependencies
```
CombatManager -> WeaponSystem, HealthSystem, DefenseSystem
WeaponSystem -> All Weapon classes
HealthSystem -> ArmorSystem
DefenseSystem -> MeleeSystem
```

### Networking Dependencies
```
NetworkManager -> PlayerSync, CombatSync, GameStateSync
PlayerSync -> Combat system files
CombatSync -> Weapon classes
GameStateSync -> Game mode scenes
```

### Asset Loading Order
1. Core UI assets (splash screens, loading)
2. Character base sprites and animations
3. Weapon sprites and effects
4. Map tiles and environmental objects
5. Audio files and sound effects
6. Particle effects and lighting

This comprehensive reference ensures every file has a clear purpose and developers understand the relationships between different systems in the project.