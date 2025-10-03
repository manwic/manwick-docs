
# Manvik - Unity C# Project Architecture

## Project Structure

```
Manvik/
├── Assets/
│   ├── _Project/                      
│   │   ├── Scripts/                   
│   │   │   ├── Core/                  
│   │   │   ├── Player/                
│   │   │   ├── Roles/                 
│   │   │   ├── Factory/               
│   │   │   ├── Tasks/                 
│   │   │   ├── Meetings/              
│   │   │   ├── UI/                    
│   │   │   ├── Networking/            
│   │   │   ├── Audio/                 
│   │   │   ├── Data/                  
│   │   │   └── Utils/                 
│   │   ├── Prefabs/                   
│   │   ├── Scenes/                    
│   │   ├── Materials/                 
│   │   ├── Sprites/                   
│   │   ├── Audio/                     
│   │   ├── Animations/                
│   │   └── Resources/                 
│   │
│   ├── Plugins/                       
│   ├── StreamingAssets/               
│   └── Settings/                      
│
├── Packages/                          
├── ProjectSettings/                   
└── UserSettings/                      
```

---

## Core Architecture Principles

### 1. **Separation of Concerns**

* Each script has a single, well-defined responsibility
* UI logic separated from game logic
* Network code isolated from gameplay code

### 2. **SOLID Principles**

* **S**ingle Responsibility
* **O**pen/Closed (extendable, not modifiable)
* **L**iskov Substitution (role inheritance)
* **I**nterface Segregation (specific interfaces)
* **D**ependency Inversion (depend on abstractions)

### 3. **Design Patterns**

* **Singleton**: GameManager, AudioManager
* **Factory**: Role creation, task creation
* **Observer**: Event system for communication
* **State Machine**: Game states, player states
* **Object Pool**: Prefab pooling for performance
* **Command**: Action recording for replays

### 4. **Code Standards**

```csharp
// Naming Conventions:
// - Classes: PascalCase (PlayerController)
// - Methods: PascalCase (InitializePlayer)
// - Private fields: _camelCase (_playerData)
// - Public properties: PascalCase (PlayerHealth)
// - Constants: UPPER_SNAKE_CASE (MAX_PLAYERS)
// - Interfaces: IPascalCase (IRole)

// Documentation:
// - All public APIs documented with XML comments
// - Complex logic explained with inline comments
// - File headers with purpose and author
```

---

## Key Systems Overview

### 1. Game Flow Manager

```csharp
public class GameManager : MonoBehaviour
{
    public static GameManager Instance { get; private set; }
    private GameState _currentState;

    public void StartGame() { }
    public void StartDiscussion() { }
    public void StartVoting() { }
    public void EndGame() { }
}
```

### 2. Role System

```csharp
public interface IRole
{
    string RoleName { get; }
    RoleType Type { get; }
    void Initialize();
    void UseAbility();
    bool CanUseAbility();
}

public abstract class RoleBase : MonoBehaviour, IRole { }
public class HumanWorker : RoleBase { }
```

### 3. Factory System Manager

```csharp
public class FactorySystem : MonoBehaviour
{
    private Dictionary<SystemType, SystemHealth> _systems;

    public void DamageSystem(SystemType type, float damage) { }
    public void RepairSystem(SystemType type, float amount) { }
    public float GetSystemHealth(SystemType type) { }
}
```

### 4. Network Architecture

```csharp
public class NetworkManager : MonoBehaviour
{
    public void HostGame() { }
    public void JoinGame(string ip) { }
    public void SyncPlayerData() { }
    public void SendRPC(string methodName, params object[] args) { }
}
```

---

## Development Workflow

### Phase 1: Foundation

* [ ] Project setup and architecture
* [ ] Core managers (Game, Network, Audio)
* [ ] Basic player movement
* [ ] Scene management
* [ ] Event system

### Phase 2: Role System

* [ ] Role interface and base class
* [ ] Human Worker implementation
* [ ] Manvik Guardian implementation
* [ ] Corrupted Machine implementation
* [ ] Role assignment system

### Phase 3: Factory Systems

* [ ] System health management
* [ ] Repair task system
* [ ] Sabotage mechanics
* [ ] Emergency events
* [ ] Visual feedback

### Phase 4: Social Features

* [ ] Meeting system
* [ ] Voting mechanics
* [ ] Chat system (text/voice)
* [ ] Player reporting
* [ ] Discussion timer

### Phase 5: Networking

* [ ] Server-client setup
* [ ] Player synchronization
* [ ] State synchronization
* [ ] Lag compensation
* [ ] Anti-cheat measures

### Phase 6: Polish

* [ ] UI/UX refinement
* [ ] Audio implementation
* [ ] Performance optimization
* [ ] Bug fixing
* [ ] Testing and balancing

---

## Git Workflow

### Branch Strategy

```
main                    # Production-ready code
├── develop             # Integration branch
├── feature/player      # Feature branches
├── feature/networking
├── bugfix/issue-123    # Bug fixes
└── hotfix/critical     # Critical fixes
```

### Commit Standards

```bash
# Format: <type>(<scope>): <subject>

feat(player): add player movement system
fix(network): resolve connection timeout
docs(readme): update architecture diagram
refactor(roles): optimize role assignment
test(factory): add system health tests
```

### Pull Request Process

1. Create feature branch from `develop`
2. Implement feature with tests
3. Submit PR with detailed description
4. Code review by team member
5. Address review comments
6. Merge after approval

---

## Code Quality Standards

### 1. Code Review Checklist

* [ ] Follows naming conventions
* [ ] No hardcoded values (use constants)
* [ ] Proper error handling
* [ ] XML documentation for public APIs
* [ ] No unused code or imports
* [ ] Optimized performance
* [ ] Memory leak prevention

### 2. Testing Requirements

* Unit tests for core systems
* Integration tests for workflows
* Network stress testing
* Cross-platform testing
* Performance profiling

### 3. Documentation

* README for each major system
* API documentation auto-generated
* Architecture diagrams updated
* Code comments for complex logic

---

## Performance Guidelines

### Optimization Targets

* **FPS**: 60 FPS on minimum specs
* **Load Time**: < 30 seconds
* **Memory**: < 2GB on mobile
* **Network**: < 100ms latency
* **Build Size**: < 1GB total

### Best Practices

* Object pooling for frequent spawns
* Sprite atlases for reduced draw calls
* Async loading for scenes
* Event-driven architecture
* Proper garbage collection management

---

## Security & Anti-Cheat

### Server Authority

* All game state on server
* Client sends inputs only
* Server validates all actions
* No sensitive data on client

### Cheat Prevention

* Server-side validation
* Encrypted network traffic
* Rate limiting on actions
* Replay system for analysis
* Report system for players

---

## Next Steps

1. **Setup Unity Project**

   * Unity version: 2022.3 LTS
   * Configure project settings
   * Import essential packages

2. **Create Core Managers**

   * GameManager singleton
   * Scene management
   * Event system

3. **Setup Version Control**

   * Initialize Git repository
   * Configure .gitignore
   * Setup branch protection

4. **Begin Development**

   * Follow phase roadmap
   * Regular code reviews
   * Continuous testing

---

