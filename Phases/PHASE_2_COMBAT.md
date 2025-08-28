e# Phase 2: Combat Core Tasks

## Stage 1: Combat Foundation
### Sprint A: Combat System Architecture
- [ ] Create CombatManager class
- [ ] Implement damage calculation system
- [ ] Create health management system (150 HP base)
- [ ] Set up team-based damage rules
- [ ] Implement death and respawn system

### Sprint B: Crosshair System
- [ ] Create crosshair rendering system
- [ ] Implement crosshair positioning
- [ ] Add crosshair customization options
- [ ] Create aim direction calculation
- [ ] Test crosshair accuracy feedback

### Sprint C: Basic Shooting
- [ ] Implement basic shooting mechanics
- [ ] Create bullet trajectory system
- [ ] Add hit detection (hitscan)
- [ ] Implement shooting sound effects
- [ ] Test basic combat interaction

## Stage 2: Weapon System Foundation
### Sprint A: Weapon Architecture
- [ ] Create Weapon base class
- [ ] Implement weapon switching system
- [ ] Create weapon attachment system
- [ ] Set up weapon upgrade pipeline
- [ ] Add weapon UI integration

### Sprint B: Primary Weapons - Assault Rifles
- [ ] Implement AK-47 style weapon
  - [ ] 35 damage, 600 RPM, 30 rounds
  - [ ] High recoil pattern
- [ ] Implement M4 style weapon
  - [ ] 30 damage, 750 RPM, 30 rounds
  - [ ] Medium recoil pattern
- [ ] Test assault rifle balance

### Sprint C: Primary Weapons - SMGs & Shotguns
- [ ] Implement MP5 style SMG
  - [ ] 25 damage, 900 RPM, 30 rounds
- [ ] Implement Pump Shotgun
  - [ ] 120 damage, 60 RPM, 8 shells
  - [ ] Spread pattern system
- [ ] Test close-range combat balance

## Stage 3: Advanced Weapons
### Sprint A: Sniper & Pistol Systems
- [ ] Implement Bolt Action Sniper
  - [ ] 120 damage, 40 RPM, 5 rounds
  - [ ] 2x zoom scope system
- [ ] Implement Standard Pistol
  - [ ] 40 damage, 300 RPM, 12 rounds
- [ ] Test long-range and backup weapons

### Sprint B: Recoil & Accuracy Systems
- [ ] Create recoil pattern system
- [ ] Implement accuracy modifiers
  - [ ] Standing: 100%, Walking: 85%, Running: 65%
- [ ] Add damage falloff over distance
- [ ] Create recoil recovery system
- [ ] Test shooting accuracy balance

### Sprint C: Weapon Audio & Visual
- [ ] Add weapon-specific sound effects
- [ ] Create muzzle flash effects
- [ ] Implement shell ejection animations
- [ ] Add weapon reload animations
- [ ] Test audio-visual feedback

## Stage 4: Health & Armor Systems
### Sprint A: Health Management
- [ ] Implement health bar UI
- [ ] Create damage number display
- [ ] Add health regeneration (if applicable)
- [ ] Implement death state handling
- [ ] Test health system integration

### Sprint B: Armor System
- [ ] Create Light Armor (+25 HP, -10% speed)
- [ ] Create Heavy Armor (+50 HP, -20% speed)
- [ ] Implement armor pickup system
- [ ] Add armor UI indicators
- [ ] Test armor balance

### Sprint C: Healing System
- [ ] Create Med Kit system (50 HP, 3-second use)
- [ ] Implement healing UI progress bar
- [ ] Add healing sound effects
- [ ] Create Shield system (25 HP regenerating)
- [ ] Test healing balance and timing

## Stage 5: Defensive Mechanics
### Sprint A: Cover System
- [ ] Implement wall collision detection
- [ ] Create cover mechanics
- [ ] Add bullet-to-wall collision
- [ ] Implement destructible cover (optional)
- [ ] Test cover effectiveness

### Sprint B: Dodge Roll System
- [ ] Create dodge roll animation
- [ ] Implement 3-second cooldown
- [ ] Add 0.2-second invincibility frames
- [ ] Create dodge roll distance (2 character lengths)
- [ ] Test dodge mechanics balance

### Sprint C: Crouching & Leaning
- [ ] Implement crouching mechanics
- [ ] Reduce hitbox size when crouching
- [ ] Add leaning around corners
- [ ] Implement accuracy bonuses for crouching
- [ ] Test defensive positioning

## Stage 6: Melee Combat
### Sprint A: Hand-to-Hand Combat
- [ ] Implement punch attack (25 damage, 1s cooldown)
- [ ] Implement kick attack (35 damage, 1.5s cooldown)
- [ ] Create grapple system (40 damage, 1s stun)
- [ ] Add melee range detection
- [ ] Test hand-to-hand balance

### Sprint B: Melee Weapons
- [ ] Implement Knife (60 damage, 0.8s cooldown)
- [ ] Implement Baseball Bat (80 damage, 1.2s cooldown)
- [ ] Implement Sword (90 damage, 1.5s cooldown)
- [ ] Create melee weapon switching
- [ ] Test melee weapon balance

### Sprint C: Melee Polish
- [ ] Add melee attack animations
- [ ] Create melee impact effects
- [ ] Implement melee sound effects
- [ ] Add melee combo system (optional)
- [ ] Test melee vs ranged balance

## Stage 7: Equipment System
### Sprint A: Throwable Grenades
- [ ] Implement Frag Grenade
  - [ ] 100 direct damage, 50 splash
  - [ ] 3-second timer, 3 character radius
- [ ] Create grenade trajectory preview
- [ ] Add grenade explosion effects
- [ ] Test grenade balance

### Sprint B: Utility Grenades
- [ ] Implement Flashbang
  - [ ] 2-second blind effect, 4 character radius
- [ ] Implement Smoke Grenade
  - [ ] 10-second vision block, 5 character radius
- [ ] Create visual effect systems
- [ ] Test utility grenade effectiveness

### Sprint C: Equipment Management
- [ ] Create equipment inventory system
- [ ] Implement equipment pickup system
- [ ] Add equipment UI indicators
- [ ] Create equipment respawn system
- [ ] Test equipment distribution balance

## Stage 8: Combat Polish & Testing
### Sprint A: Combat Balance
- [ ] Fine-tune all weapon damages
- [ ] Adjust health and armor values
- [ ] Balance movement speeds
- [ ] Test time-to-kill ratios
- [ ] Conduct combat playtesting

### Sprint B: Visual Polish
- [ ] Add hit markers and damage indicators
- [ ] Implement kill feed system
- [ ] Create combat UI elements
- [ ] Add combat screen effects
- [ ] Test visual feedback clarity

### Sprint C: Integration & Testing
- [ ] Integrate all combat systems
- [ ] Create combat test scenarios
- [ ] Performance testing under combat load
- [ ] Bug fixing and optimization
- [ ] Prepare for Phase 3 development

## 📋 Phase 2 Deliverables
- ✅ Complete weapon system (5 primary weapons)
- ✅ Health, armor, and damage systems
- ✅ Defensive mechanics (cover, dodge, crouch)
- ✅ Melee combat system
- ✅ Equipment system (grenades, healing)
- ✅ Balanced combat gameplay

## 🎯 Success Criteria
- All weapons feel distinct and balanced
- Combat is skill-based and engaging
- Health/armor system promotes strategic play
- Defensive options provide tactical depth
- Equipment adds strategic variety to gameplay