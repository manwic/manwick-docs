# Project Description
The 2D Tactical Team Shooter is a fast-paced multiplayer game that emphasizes team coordination, tactical movement, and strategic combat. Unlike traditional shooters that prioritize raw reflexes, this game focuses on cooperative gameplay, where players take on different roles and use weapons, gadgets, and abilities to secure victory.

Players compete in teams across objective-based maps (Capture the Flag, Secure Zone, Elimination) with a top-down 2D perspective. The project is built using a modern 2D game engine and supports real-time multiplayer networking, customizable loadouts, and tactical gadgets.


# Manwick Documentation Hub

Comprehensive documentation for Manwick tactical shooter development.

## Overview

<img width="5327" height="7786" alt="mindmap-manvik" src="https://github.com/user-attachments/assets/a43ad8c4-d152-4aca-89a6-640d1939b5de" />


This repository contains all documentation for the Manwick project, including game design documents, technical specifications, development guides, and community resources.

## Documentation Structure

### Game Design
- [Master Task List](GameDesign/MASTER_TASK_LIST.md) - Complete development roadmap
- [Game Design Document](https://github.com/manwic/manwick-docs/blob/main/GAME_DESIGN_DOCUMENT.md) - Core game specifications
- [Technical Specifications](GameDesign/TECHNICAL_SPECIFICATIONS.md) - System requirements and tech details

### Development Guides  
- [Getting Started](Development/GETTING_STARTED.md) - Setup and development workflow
- [Code Reference](Development/CODE_REFERENCE.md) - File structure and code purposes
- [Build Instructions](Development/BUILD_INSTRUCTIONS.md) - How to build the Sure! Here's a refined list of the **best usage example points** for a 2D tactical shooter game (like the one you described), focusing on **clarity**, **structure**, and **real-world relevance** for players and testers:

---

### ✅ **Best Points for Usage Example – 2D Shooter Game**

---

#### 🔹 **1. Starting the Game**

* **Host a Game (Server Mode):**

  ```bash
  ./tactical-shooter.exe --host
  ```

  > Starts a local server allowing other players to connect to your machine.

* **Join a Game (Client Mode):**

  ```bash
  ./tactical-shooter.exe --connect 192.168.1.100
  ```

  > Connects to a host machine (replace with actual IP of host).

---

#### 🔹 **2. Match Setup Flow**

1. **Player A** hosts the match.
2. **Players B, C, etc.** join using the host’s IP.
3. Game auto-assigns players to **Red** or **Blue** team.
4. Each player selects a **loadout**:

   * Rifleman (assault-focused)
   * Sniper (long-range)
   * Medic (support & healing)

---

#### 🔹 **3. Gameplay Objectives**

* Red Team: **Defend** the base.
* Blue Team: **Attack** to capture the flag.
* First team to win **3 rounds** wins the match.

---

#### 🔹 **4. Core Controls**

| Action      | Key/Button |
| ----------- | ---------- |
| Move        | `W A S D`  |
| Aim & Shoot | `Mouse`    |
| Reload      | `R`        |
| Use Gadget  | `Q / E`    |
| Scoreboard  | `Tab`      |
| Pause/Menu  | `Esc`      |

---

#### 🔹 **5. Quick Gameplay Tips**

* **Use cover** to avoid incoming fire.
* **Coordinate** with your team using roles (e.g. sniper covers, medic supports).
* **Flank** the enemy to break defensive lines.
* **Watch reload timing** – don’t reload in open ground.

---

#### 🔹 **6. Example Scenario**

> **You** host the match.
> **Your friends** join your IP.
> You play as a **Medic on Red Team**, defending base with gadgets.
> A teammate (Sniper) covers the flag.
> You win 3 rounds by defending successfully – **Victory!**

---


- [Contributing Guidelines](Development/CONTRIBUTING.md) - How to contribute to development

### Phase Documentation
- [Phase 1: Foundation](Phases/PHASE_1_FOUNDATION.md) [COMPLETE]
- [Phase 2: Combat Core](Phases/PHASE_2_COMBAT.md) [IN PROGRESS]  
- [Phase 3: Maps & Environment](Phases/PHASE_3_MAPS.md) [PLANNED]
- [Phase 4: Game Modes](Phases/PHASE_4_GAMEMODES.md) [PLANNED]
- [Phase 5: Multiplayer](Phases/PHASE_5_MULTIPLAYER.md) [PLANNED]
- [Phase 6: Polish & Systems](Phases/PHASE_6_POLISH.md) [PLANNED]

### API Documentation
- [Core Systems API](API/CORE_SYSTEMS.md) - Core game systems
- [Combat System API](API/COMBAT_SYSTEM.md) - Combat mechanics
- [Networking API](API/NETWORKING.md) - Multiplayer systems
- [UI System API](API/UI_SYSTEM.md) - User interface

### Community Resources
- [Modding Guide](Community/MODDING_GUIDE.md) - How to create mods
- [Map Creation](Community/MAP_CREATION.md) - Custom map development  
- [Asset Guidelines](Community/ASSET_GUIDELINES.md) - Art and asset standards
- [Community Events](Community/EVENTS.md) - Community challenges and events

## Quick Links

### For Developers
- **[Getting Started Guide](Development/GETTING_STARTED.md)** - Start here
- **[Master Task List](GameDesign/MASTER_TASK_LIST.md)** - Full development plan
- **[Code Reference](Development/CODE_REFERENCE.md)** - File structure guide

### For Contributors  
- **[Contributing Guidelines](Development/CONTRIBUTING.md)** - How to help
- **[Code of Conduct](Development/CODE_OF_CONDUCT.md)** - Community standards
- **[Issue Templates](Development/ISSUE_TEMPLATES.md)** - Bug reports and features

### For Community
- **[Modding Guide](Community/MODDING_GUIDE.md)** - Create custom content
- **[Community Hub](Community/COMMUNITY_HUB.md)** - Community resources
- **[FAQ](Community/FAQ.md)** - Frequently asked questions

## Repository Links

- **[Main Game Repository](https://github.com/manwic/manwick)** - Complete game source code
- **[Development Tools](https://github.com/manwic/manwick-tools)** - Custom dev tools  
- **[Community Hub](https://github.com/manwic/manwick-community)** - User content
- **[Game Server](https://github.com/manwic/manwick-server)** - Multiplayer infrastructure

## Development Status

### Current Phase: Combat Core Development
- **Overall Progress**: Phase 1 Complete, Phase 2 Active
- **Active Tasks**: Weapon systems, combat mechanics, health systems
- **Next Milestone**: Complete weapon implementation
- **Documentation Status**: All phases documented and ready

### Recent Updates
- ✅ Complete project structure established
- ✅ Comprehensive task breakdowns created  
- ✅ Professional documentation system implemented
- 🔄 Combat system development beginning

## Contributing to Documentation

We welcome contributions to improve our documentation:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b improve-docs`)
3. **Make your changes** (improve clarity, fix typos, add examples)
4. **Test your changes** (check all links work)
5. **Submit a pull request** with clear description

### Documentation Standards
- Use clear, concise language
- Include code examples where relevant
- Maintain consistent formatting
- Update table of contents when adding new sections
- Test all links before submitting

## License

This documentation is licensed under [MIT License](LICENSE).

---

**Manwick Team** | [Website](https://manwick.game) | [Community Discord](https://discord.gg/RP6efE4u)
