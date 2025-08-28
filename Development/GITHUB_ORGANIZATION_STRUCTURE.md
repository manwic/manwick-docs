# GitHub Organization Structure Plan

## Organization: https://github.com/manwic

Complete organizational structure for the Manwick tactical shooter project and future game development.

## Repository Structure

### Core Game Repositories

#### 1. `manwick` (Main Game Repository)
**Purpose**: Complete game source code and development
**Contents**:
- Complete LibGDX source code
- All game assets (characters, weapons, maps)
- Build configurations for all platforms
- Development documentation
- Issue tracking for bugs and features

#### 2. `manwick-docs` (Documentation Hub)
**Purpose**: Comprehensive project documentation
**Contents**:
- Game design documents
- Technical specifications
- Development guides and tutorials
- API documentation
- Contributing guidelines
- Community resources

#### 3. `manwick-assets` (Asset Repository)
**Purpose**: Raw assets and asset pipeline
**Contents**:
- Source art files (.psd, .ai, .sketch)
- Audio source files
- 3D models and textures
- Asset creation guidelines
- Asset pipeline tools

### Development Tools & Infrastructure

#### 4. `manwick-tools` (Development Tools)
**Purpose**: Custom development tools and utilities
**Contents**:
- Map editor tools
- Asset processing scripts
- Build automation tools
- Testing utilities
- Performance profiling tools

#### 5. `manwick-server` (Game Server)
**Purpose**: Multiplayer server infrastructure
**Contents**:
- Dedicated server code
- Matchmaking system
- Anti-cheat systems
- Server management tools
- Deployment scripts

#### 6. `manwick-launcher` (Game Launcher)
**Purpose**: Game launcher and updater
**Contents**:
- Cross-platform launcher
- Auto-update system
- User authentication
- News and announcements
- Settings management

### Platform-Specific Repositories

#### 7. `manwick-desktop` (Desktop Platform)
**Purpose**: Desktop-specific implementations
**Contents**:
- Windows/Mac/Linux builds
- Platform-specific features
- Steam integration (future)
- Desktop launcher

#### 8. `manwick-mobile` (Mobile Platform - Future)
**Purpose**: Mobile port development
**Contents**:
- Mobile-optimized UI
- Touch controls
- Mobile-specific features
- App store configurations

### Community & Resources

#### 9. `manwick-community` (Community Hub)
**Purpose**: Community resources and contributions
**Contents**:
- Community maps and mods
- User-generated content guidelines
- Community challenges
- Fan art and resources

#### 10. `manwick-website` (Official Website)
**Purpose**: Official game website
**Contents**:
- Marketing website
- Player statistics
- News and updates
- Download links
- Community forums integration

## Organization Settings

### Team Structure

#### Core Development Team
- **Owner**: Full access to all repositories
- **Lead Developer**: Core game development
- **Art Director**: Asset creation and management
- **Backend Developer**: Server and infrastructure

#### Community Team
- **Community Manager**: Community repositories
- **Moderators**: Issue management and community support
- **Contributors**: External contributors with limited access

### Repository Permissions

#### Public Repositories
- `manwick` - Public (for community visibility)
- `manwick-docs` - Public (for documentation access)
- `manwick-community` - Public (for community contributions)
- `manwick-website` - Public (for transparency)

#### Private Repositories (Development)
- `manwick-server` - Private (security reasons)
- `manwick-assets` - Private (source assets)
- `manwick-tools` - Private (internal tools)

## Setup Instructions

### Phase 1: Core Repositories
1. **Create Main Repository**
   ```bash
   # Current: manwick (already exists)
   # Move existing code here
   ```

2. **Create Documentation Repository**
   ```bash
   # Create: manwick-docs
   # Move Documentation/ folder here
   ```

3. **Create Assets Repository**
   ```bash
   # Create: manwick-assets
   # Set up LFS for large files
   ```

### Phase 2: Development Infrastructure
4. **Create Tools Repository**
   ```bash
   # Create: manwick-tools
   # Add development utilities
   ```

5. **Create Server Repository**
   ```bash
   # Create: manwick-server
   # Private repository for server code
   ```

### Phase 3: Platform & Community
6. **Create Platform Repositories**
   ```bash
   # Create: manwick-desktop
   # Create: manwick-launcher
   ```

7. **Create Community Hub**
   ```bash
   # Create: manwick-community
   # Create: manwick-website
   ```

## Repository Templates

### Standard Files for Each Repository
- `README.md` - Repository overview
- `LICENSE` - Software license
- `CONTRIBUTING.md` - Contribution guidelines
- `CODE_OF_CONDUCT.md` - Community standards
- `.gitignore` - Repository-specific ignores
- `CHANGELOG.md` - Version history

### Branch Protection Rules
- **main**: Protected, requires PR reviews
- **develop**: Active development branch
- **release/***: Release preparation branches
- **feature/***: Feature development branches

## GitHub Organization Features

### Project Boards
- **Game Development**: Overall project tracking
- **Community**: Community-related tasks
- **Infrastructure**: Server and tools development

### Team Management
- **@manwic/core**: Core development team
- **@manwic/community**: Community management
- **@manwic/contributors**: External contributors

### Security & Access
- **Two-factor authentication**: Required for all team members
- **Dependency scanning**: Automated security checks
- **Secret scanning**: Prevent credential leaks

## Integration Setup

### Continuous Integration
- **GitHub Actions**: Automated testing and builds
- **Automated releases**: Version tagging and releases
- **Cross-platform builds**: Windows, Mac, Linux

### External Integrations
- **Discord**: Community notifications
- **Website**: Automatic updates
- **Analytics**: Development metrics

## Migration Plan

### Current State to Organization Structure

#### Week 1: Foundation
- Set up organization structure
- Create core repositories
- Migrate existing documentation

#### Week 2: Development Setup
- Create development repositories
- Set up CI/CD pipelines
- Configure team permissions

#### Week 3: Community Setup
- Create community repositories
- Set up project boards
- Configure integrations

#### Week 4: Launch & Polish
- Finalize all repositories
- Test all integrations
- Launch organization publicly

## Repository Descriptions

### Main Repositories
```
manwick: "2D top-down tactical team shooter with 4v4 combat and strategic depth"
manwick-docs: "Comprehensive documentation for Manwick game development"
manwick-server: "Multiplayer server infrastructure for Manwick"
manwick-tools: "Development tools and utilities for Manwick"
```

### Supporting Repositories
```
manwick-assets: "Source assets and asset pipeline for Manwick"
manwick-launcher: "Cross-platform game launcher and updater"
manwick-community: "Community resources, maps, and user-generated content"
manwick-website: "Official Manwick game website"
```

This structure provides:
- ✅ Organized development workflow
- ✅ Clear separation of concerns
- ✅ Community engagement opportunities
- ✅ Scalable infrastructure
- ✅ Professional project presentation
- ✅ Future expansion capability