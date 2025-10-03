# Game Design Document (GDD)


## Manvik - 2D Social Deduction Game

---

## Document Information
- **Version**: 1.1
- **Date**: septmber 26, 2025
- **Author**: Manish Rathaur
- **Team**: [kapil]
- **Status**: In Development

---

## 1. Executive Summary

### Game Overview
**Game Title**: Manvik  
**Genre**: Social Deduction, Multiplayer, Strategy, Sci-Fi  
**Platform**: Windows & Android  
**Target Audience**: 13-35 years old, casual to moderate gamers  
**Player Count**: 6-8 players per game  
**Development Time**: 12-18 months  
**Team Size**: [To be determined]

### Core Game Loop
1. **Lobby Phase**: Players join and customize characters/units
2. **Role Assignment**: Secret distribution of Human Workers, Manvik Guardians, or Corrupted Machines
3. **Gameplay Phase**: Complete repairs while identifying corrupted machines or sabotage systems
4. **Emergency Phase**: Crisis events, meetings, and voting
5. **Resolution Phase**: Victory/defeat based on faction objectives

### Unique Selling Points (USP)
- **Three-faction system**: Unique dynamic beyond traditional impostor/crewmate
- **Factory system status**: Health percentages affecting gameplay
- **Cross-platform play**: PC and mobile players in the same games
- **Sci-fi narrative**: Engaging storyline with purpose
- **Guardian mechanics**: Manvik units with protective abilities
- **Accessibility features**: Colorblind support, text-to-speech

---

## 2. Game Vision & Design Pillars

### Vision Statement
*"Create an immersive sci-fi social deduction experience with strategic depth that connects players across platforms through the Manvik universe."*

### Design Pillars

#### 1. Narrative Integration
- Story-driven gameplay with purpose
- Thematic consistency across all elements
- Lore development through environmental storytelling
- Character roles with narrative justification

#### 2. Strategic Depth
- Three distinct factions with unique win conditions
- System health management affecting game state
- Guardian protection mechanics
- Emergency event coordination requirements

#### 3. Cross-Platform Accessibility
- Seamless PC and mobile integration
- Control schemes optimized for each platform
- Consistent performance across devices
- Shared progression and cosmetics

#### 4. Community Engagement
- Built-in communication tools
- Streamer-friendly features
- User-generated content potential
- Regular content updates

---

## 3. Target Audience Analysis

### Primary Audience (65%)
- **Age**: 16-28 years old
- **Gaming Experience**: Casual to moderate
- **Platforms**: Multi-platform (PC and mobile)
- **Play Style**: Social, narrative-driven, 15-30 minute sessions
- **Motivation**: Sci-fi themes, social interaction, strategic gameplay

### Secondary Audience (25%)
- **Age**: 29-35 years old
- **Gaming Experience**: Moderate to hardcore
- **Platforms**: PC-primary
- **Play Style**: Strategic, team coordination, 30-45 minute sessions
- **Motivation**: Complex mechanics, competitive play, depth

### Tertiary Audience (10%)
- **Age**: 13-15 years old
- **Gaming Experience**: Varies
- **Platforms**: Mobile-primary
- **Play Style**: Casual, social
- **Motivation**: Following trends, peer activities

---

## 4. Core Gameplay Mechanics

### 4.1 Player Roles

#### Human Workers (60% of players)
**Objective**: Repair all factory systems OR identify and eliminate all corrupted machines

**Abilities**:
- Repair damaged factory systems through mini-games
- Call emergency meetings when threats are discovered
- Access security terminals to monitor factory status
- Coordinate with Manvik Guardian Units for protection

**Key Tasks**:
- Repair conveyor belts and production lines
- Reboot control systems and computers
- Restore power grid functionality
- Fix medical bay life support systems
- Repair communication arrays

**Win Conditions**:
- All factory systems reach 100% operational status
- All corrupted machines are identified and eliminated
- Factory achieves "Safe Mode" with contained corruption

#### Manvik Guardian Units (25% of players)
**Primary Objective**: Protect human workers AND eliminate all corrupted machines

**Abilities**:
- Engage and eliminate corrupted machines when detected
- Activate shield mode to protect nearby humans
- Use limited scans to detect suspicious behavior
- Move efficiently on patrol routes between critical areas

**Key Tasks**:
- Maintain perimeter security at entrances and exits
- Scan facility areas for corruption signatures
- Provide emergency response during crises
- Assist with medical emergencies

**Win Conditions**: Same as Human Workers (allied victory)

#### Corrupted Machines (15% of players)
**Primary Objective**: Eliminate all humans OR sabotage enough systems to destroy the factory

**Abilities**:
- Appear as normal Helper Bots until taking hostile action
- Sabotage factory systems to spread chaos
- Eliminate humans and Guardian Bots secretly
- Access maintenance tunnels for quick movement
- Spread virus to convert eliminated players (special game modes)

**Win Conditions**:
- All human players are eliminated
- Critical factory systems are destroyed beyond repair
- Corruption spreads to 75% of facility systems

### 4.2 Factory System Status

The factory operates five critical systems that determine game state:

1. **Power Grid**: Controls lighting and player visibility
2. **Production Line**: Affects human victory conditions
3. **Security Network**: Influences Manvik Guardian Unit effectiveness
4. **Life Support**: Critical for human player survival
5. **Central AI**: Prevents corruption from spreading

Each system has health percentages that affect gameplay. Systems below 25% health trigger emergency situations.

### 4.3 Sabotage System

#### Sabotage Types
| Sabotage | Effect | Countdown | Strategy |
|----------|--------|-----------|----------|
| **Reactor Overload** | Critical system failure | 30 seconds | Forces grouping |
| **Power Grid Failure** | Reduces vision radius | None | Isolation plays |
| **Security Lockdown** | Locks specific rooms | 15 seconds | Trap players |
| **Communication Jam** | Disables task list | None | Information denial |
| **Production Damage** | Harms manufacturing | None | Slows progress |

### 4.4 Voting & Discussion System

#### Meeting Types
- **Emergency Meeting**: Called by any living player (limited uses)
- **Body Report**: Triggered when finding eliminated player
- **System Critical**: Automatic meeting during critical system failures

#### Voting Mechanics
- **Anonymous Voting**: Players don't see who voted for whom until results
- **Role-Specific Voting**: Manvik Guardians may have additional voting powers
- **Majority Rules**: Most votes determines elimination
- **Tie Rules**: No elimination on ties
- **Skip Vote**: Option to not eliminate anyone
- **Discussion Time**: 30-120 seconds (customizable)
- **Voting Time**: 15-60 seconds (customizable)

---

## 5. Game Flow & Progression

### 5.1 Match Structure

### 5.2 Session Progression

#### Pre-Game (2-5 minutes)
- **Lobby Setup**: Host configures rules and map
- **Player Joining**: 6-12 players join
- **Customization**: Character/unit appearance options
- **Ready Check**: All players confirm readiness

#### Main Game (8-20 minutes)
- **Role Distribution**: Secret assignment of three factions
- **Gameplay Loop**: Repairs, protection, sabotage, meetings
- **Dynamic Events**: System failures and emergencies
- **Social Interaction**: Communication and deduction

#### Post-Game (1-3 minutes)
- **Results Screen**: Winning faction, statistics, MVP
- **Performance Review**: Systems repaired, eliminations, accuracy
- **Social Features**: Friend requests, ratings
- **Lobby Return**: Option to play again with same group

---

## 6. User Interface Design

### 6.1 UI Hierarchy

#### Main Menu
- **Play Button**: Quick match or lobby browser
- **Create Lobby**: Host private games
- **Settings**: Graphics, audio, controls
- **Store**: Cosmetics and customization
- **Profile**: Stats, achievements, friends
- **Lore**: Story and character information

#### In-Game UI
- **System Status Panel**: Health of all factory systems
- **Task List**: Current repair objectives (humans only)
- **Mini-Map**: Room layout and player positions
- **Ability Cooldowns**: Special power indicators
- **Report Button**: Report eliminated players
- **Emergency Button**: Call meetings (limited uses)
- **Sabotage Menu**: Available sabotages (corrupted only)

#### Meeting UI
- **Player Grid**: All living players with voting buttons
- **Chat Window**: Text communication during discussion
- **System Status**: Current factory condition display
- **Timer Display**: Countdown for discussion/voting phases
- **Role Reveal**: Limited information based on player role

### 6.2 Mobile-Specific UI

#### Touch Controls
- **Virtual Joystick**: Movement control (bottom-left)
- **Action Buttons**: Use, Report, Emergency (bottom-right)
- **Task Interface**: Touch-optimized repair mini-games
- **Voting Interface**: Large, finger-friendly buttons

#### Screen Adaptation
- **Portrait Mode**: Optimized for phone screens
- **Landscape Mode**: Tablet-friendly layout
- **Dynamic UI**: Scales with screen size
- **Safe Areas**: Respect notches and navigation bars

---

## 7. Art & Audio Direction

### 7.1 Visual Style

#### Art Style
- **2D Top-Down**: Functional perspective for gameplay
- **Cyberpunk Industrial**: Clean futuristic factory aesthetic
- **Color Coding**: Role-specific visual identifiers
- **Corruption Effects**: Visual distortion for corrupted units
- **Scalable Graphics**: Works on all screen sizes

#### Character Design
- **Human Workers**: Professional technical uniforms with tools
- **Manvik Guardians**: Military-inspired robotic designs
- **Corrupted Machines**: Glitching, sparking versions of helper bots
- **Cosmetic Options**: Helmets, toolkits, armor variants, LED patterns
- **Animation States**: Idle, walking, repairing, combat stances

#### Environment Design
- **Factory Omega-7 Setting**: Modular industrial environments
- **System-Specific Areas**: Distinct visual design for each system
- **Corruption Spread**: Visual indicators of system degradation
- **Emergency States**: Flashing lights, alarm indicators, smoke effects

### 7.2 Audio Design

#### Sound Effects
- **Factory Ambiance**: Machinery hums, conveyor operations
- **Role-Specific Sounds**: Repair tools, robotic movements, corruption effects
- **System Alerts**: Distinct audio for each emergency type
- **UI Sounds**: Futuristic interface feedback
- **Elimination Sounds**: Dramatic effects for player removal

#### Music & Ambiance
- **Lobby Music**: Atmospheric industrial themes
- **Gameplay Tension**: Building suspense based on system status
- **Emergency Music**: Intense, urgent themes during crises
- **Victory/Defeat**: Faction-specific conclusion themes
- **Adaptive Audio**: Changes based on corruption spread

#### Voice Chat Integration
- **Proximity Chat**: Hear nearby players clearly
- **Emergency Chat**: All players hear each other during crises
- **Role-Specific Channels**: Potential for faction-only communication
- **Push-to-Talk**: Optional voice activation
- **Audio Quality**: Clear, low-latency communication

---

## 8. Technical Specifications

### 8.1 Platform Requirements

#### PC Requirements
**Minimum**:
- OS: Windows 10 / macOS 10.14 / Ubuntu 18.04
- Processor: Intel i3 / AMD FX-6300
- Memory: 2 GB RAM
- Graphics: DirectX 11 compatible
- Network: Broadband Internet
- Storage: 1 GB available space

**Recommended**:
- OS: Windows 11 / macOS 12+ / Ubuntu 20.04+
- Processor: Intel i5 / AMD Ryzen 5
- Memory: 4 GB RAM
- Graphics: Dedicated graphics card
- Network: Stable broadband connection
- Storage: 2 GB available space

#### Android Requirements
**Minimum**:
- OS: Android 6.0 (API level 23)
- RAM: 2 GB
- Storage: 500 MB free space
- OpenGL ES 3.0 support
- Network: 3G/WiFi connection

**Recommended**:
- OS: Android 8.0+ (API level 26+)
- RAM: 3 GB+
- Storage: 1 GB free space
- Vulkan API support
- Network: 4G/WiFi connection

### 8.2 Network Architecture

#### Client-Server Model
- **Authoritative Server**: Prevents cheating
- **Dedicated Servers**: Stable connections
- **Regional Servers**: Reduced latency
- **Fallback System**: P2P if servers unavailable

#### Network Features
- **Cross-Platform**: PC and mobile compatibility
- **Matchmaking**: Role-balanced player matching
- **Anti-Cheat**: Server-side validation
- **Reconnection**: Rejoin dropped games
- **Spectator Mode**: Watch ongoing games

### 8.3 Data Management

#### Player Data
- **Account System**: Cross-platform profiles
- **Progress Sync**: Save games across devices
- **Statistics Tracking**: Games played, win rates by role
- **Achievement System**: Unlockable rewards
- **Privacy Controls**: Data protection compliance

#### Game Data
- **Match History**: Recent game records with role information
- **Replay System**: Review past matches
- **Factory Layouts**: Custom and official maps
- **Settings Sync**: Preferences across platforms

---

## 9. Monetization Strategy

### 9.1 Business Model

#### Free-to-Play Core
- **Base Game**: Completely free
- **All Maps**: Free access to gameplay content
- **No Pay-to-Win**: Cosmetics only
- **Fair Gameplay**: Equal opportunities for all players

#### Cosmetic Monetization
- **Character Skins**: Visual customization for each role
- **Equipment Variants**: Tools, weapons, accessories
- **Visual Effects**: Corruption patterns, guardian energy colors
- **Factory Themes**: Visual variants of factory environments
- **Victory Animations**: Special celebration effects

### 9.2 Pricing Strategy

#### Premium Currency
- **Factory Credits**: Earned through gameplay
- **Omega Coins**: Purchased with real money
- **Conversion Rate**: 100 credits = $1 equivalent
- **Daily Rewards**: Free credits for regular play

#### Cosmetic Pricing
| Item Type | Credit Cost | Coin Cost | USD Equivalent |
|-----------|-----------|----------|----------------|
| Basic Helmet | 500 credits | 50 coins | $0.50 |
| Role Skin | 1000 credits | 100 coins | $1.00 |
| Weapon Effect | 2000 credits | 200 coins | $2.00 |
| Factory Theme | 1500 credits | 150 coins | $1.50 |

### 9.3 Monetization Ethics

#### Fair Practices
- **No Loot Boxes**: Direct purchases only
- **Clear Pricing**: Transparent costs
- **Earn Through Play**: All items obtainable for free
- **No Pressure**: No mandatory purchases
- **Parental Controls**: Spending limits for minors

---

## 10. Marketing & Community

### 10.1 Launch Strategy

#### Pre-Launch (3-6 months)
- **Social Media**: Build anticipation on Twitter, TikTok, Discord
- **Influencer Partnerships**: Gaming streamers and YouTubers
- **Beta Testing**: Closed and open beta programs
- **Press Coverage**: Gaming journalism and websites

#### Launch (First month)
- **Platform Features**: Steam featured, Google Play promotion
- **Content Creator Events**: Sponsored gameplay sessions
- **Community Contests**: Fan art, video competitions
- **Launch Trailer**: Showcase gameplay and features

#### Post-Launch (Ongoing)
- **Regular Updates**: New content every 2-3 months
- **Seasonal Events**: Holiday-themed content
- **Community Engagement**: Developer livestreams, Q&As
- **Esports Support**: Tournament organization and prizes

### 10.2 Community Building

#### Official Channels
- **Discord Server**: Central hub for players
- **Reddit Community**: Discussion and feedback
- **Twitter Account**: News and updates
- **YouTube Channel**: Developer insights, tutorials

#### Community Features
- **Friend System**: Add and play with friends
- **Clan System**: Group creation and management
- **Leaderboards**: Skill rankings by role
- **User-Generated Content**: Custom maps and mods

---

## 11. Development Roadmap

### 11.1 Milestone Schedule

#### Alpha Phase (Months 1-6)
- **Core Gameplay**: Basic mechanics implemented
- **Single Factory Map**: One fully playable environment
- **Local Multiplayer**: Testing core systems
- **Basic UI**: Functional interface elements
- **Role Implementation**: All three factions functional

#### Beta Phase (Months 7-10)
- **Network Multiplayer**: Online gameplay
- **Multiple Maps**: 2-3 different factory environments
- **Full UI**: Complete interface design
- **Cross-Platform**: PC and Android builds
- **System Status Mechanics**: Health percentage systems

#### Release Candidate (Months 11-12)
- **Performance Optimization**: Smooth gameplay
- **Bug Fixes**: Address all critical issues
- **Balancing**: Fine-tune role mechanics
- **Marketing Preparation**: Trailers, press kits

#### Launch (Month 13)
- **Public Release**: Available on all platforms
- **Day-One Patch**: Address launch issues
- **Community Support**: Active monitoring and response
- **Post-Launch Content**: First update planned

### 11.2 Post-Launch Roadmap

#### Year 1 Content Plan
- **Month 1**: Launch stabilization and hotfixes
- **Month 3**: New factory map and game mode
- **Month 6**: Major feature update (spectator mode)
- **Month 9**: Holiday seasonal event
- **Month 12**: Anniversary celebration content

---

## 12. Risk Assessment

### 12.1 Technical Risks

#### High Risk
- **Network Stability**: Multiplayer synchronization issues
- **Cross-Platform**: PC/Android compatibility problems
- **Role Balance**: Three-faction equilibrium challenges
- **Performance**: Mobile device optimization challenges

#### Mitigation Strategies
- **Early Prototyping**: Test network systems first
- **Platform Testing**: Regular builds on all targets
- **Balance Research**: Extensive playtesting for role fairness
- **Device Testing**: Test on various mobile hardware

### 12.2 Market Risks

#### Competition
- **Established Games**: Among Us, Town of Salem, Werewolf
- **New Entrants**: Other developers entering market
- **Platform Changes**: Store algorithm changes
- **Trend Shifts**: Genre popularity changes

#### Differentiation Strategy
- **Unique Setting**: Sci-fi factory environment
- **Three-Faction System**: Deeper strategic possibilities
- **Narrative Integration**: Story-driven social deduction
- **Regular Updates**: Keep content fresh

### 12.3 Business Risks

#### Monetization
- **Low Conversion**: Players don't purchase cosmetics
- **Market Saturation**: Too many similar games
- **Platform Fees**: App store revenue sharing
- **Development Costs**: Budget overruns

#### Financial Planning
- **Conservative Projections**: Plan for lower revenue
- **Multiple Revenue Streams**: Diverse monetization
- **Cost Control**: Regular budget reviews
- **Investor Relations**: Clear communication about progress

---

## 13. Success Metrics

### 13.1 Key Performance Indicators (KPIs)

#### Player Engagement
- **Daily Active Users (DAU)**: Target 10,000+ after 6 months
- **Session Length**: Average 20+ minutes per session
- **Retention Rate**: 40%+ Day-7 retention
- **Games per Session**: Average 3+ matches per login

#### Technical Performance
- **Crash Rate**: <1% of all sessions
- **Load Times**: <30 seconds to join game
- **Network Latency**: <100ms for 90% of players
- **Frame Rate**: 60 FPS on target devices

#### Business Metrics
- **Conversion Rate**: 5%+ of players make purchases
- **Average Revenue Per User (ARPU)**: $2+ per month
- **Customer Acquisition Cost (CAC)**: <$5 per player
- **Lifetime Value (LTV)**: $15+ per paying user

### 13.2 Quality Assurance

#### Testing Standards
- **Functionality**: All features work as designed
- **Performance**: Meets technical requirements
- **Usability**: Intuitive and accessible interface
- **Compatibility**: Works on all target platforms
- **Security**: No exploits or cheats possible

#### Player Satisfaction
- **App Store Rating**: 4.0+ stars average
- **Review Sentiment**: 70%+ positive reviews
- **Community Feedback**: Active, constructive discussions
- **Bug Reports**: <10 critical issues per month
- **Support Response**: <24 hours average response time


### 14.3 Document Updates
This document is a living resource that will be updated throughout development. Major revisions will be tracked, and all team members will be notified of significant changes to ensure alignment on project vision and requirements.

---

**Document Status**: In Development  
**Next Review Date**: November 30, 2025  
**Approval Required From**: [manish]

---

*This Game Design Document serves as the foundational blueprint for Manvik development. All team members should reference this document regularly and propose changes through the established review process.*
