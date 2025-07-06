# Project Brief: Survivors V5 VLA

## Project Overview
**Game Name:** Survivors  
**Project Type:** Unity 2D Top-Down Survival Game  
**Architecture:** Zenject-based Dependency Injection  
**Target Platform:** Mobile (with SimpleInput for mobile controls)

## Core Gameplay
- **Genre:** Top-down survival/action game
- **Player:** Hero character with upgradable abilities
- **Enemies:** Multiple enemy types with AI behaviors
- **Combat:** Projectile-based combat system with guns
- **Progression:** Player level-up system with upgrades
- **Loot:** Experience gems and health potions
- **Difficulty:** Dynamic difficulty scaling system

## Technical Architecture

### Core Systems
- **Dependency Injection:** Zenject framework
- **Scene Management:** Bootstrap pattern with scene loading service
- **Input System:** SimpleInput for mobile-friendly controls
- **Asset Management:** Configurable asset loading system
- **UI Management:** Modular UI system with prefab-based windows

### Gameplay Systems
- **Character System:** Heroes and enemies with shared behaviors
- **Combat System:** Gun-based projectile combat
- **Movement System:** AI-driven enemy movement, player input movement
- **Loot System:** Drop-based item collection
- **Difficulty System:** Dynamic scaling based on game state
- **Team System:** Team-based identification and targeting
- **Vision System:** Enemy detection and awareness
- **Lifetime Management:** Object pooling and lifecycle management

### Code Organization
```
Assets/Code/
├── Common/           # Shared utilities and extensions
├── Gameplay/         # Core gameplay systems
│   ├── Characters/   # Hero and enemy implementations
│   ├── Combat/       # Combat behaviors and systems
│   ├── Guns/         # Weapon systems
│   ├── Movement/     # Movement behaviors
│   ├── PickUps/      # Item collection system
│   └── Projectiles/  # Projectile management
├── Infrastructure/   # Core services and DI setup
│   ├── Installers/   # Zenject installers
│   ├── Services/     # Core services (config, input, etc.)
│   └── UIManagement/ # UI factory and management
└── UI/              # UI components and windows
```

## Key Dependencies
- **Zenject:** Dependency injection framework
- **SimpleInput:** Mobile input system
- **Unity 2D:** Core 2D game development
- **Unity AI:** AI assistance and code generation

## Development Status
- **Current Phase:** Initial setup and project structure
- **Architecture:** Well-established with clear separation of concerns
- **Dependencies:** All major systems in place
- **Ready for:** Feature development and gameplay iteration

## Project Goals
1. Create engaging survival gameplay
2. Implement smooth mobile controls
3. Build scalable architecture for future features
4. Maintain clean code structure with DI patterns
5. Optimize for mobile performance

