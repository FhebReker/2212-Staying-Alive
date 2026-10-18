# COMPSCI 2212 - Introduction to Software Engineering
Course project completed for COMPSCI 2212 at Western University.

This repository contains **Staying Alive**, a Java Swing typing game developed using software engineering principles including object-oriented design, modular architecture, documentation standards, persistent data storage, automated testing, and collaborative development workflows.

The project challenges players to defeat incoming enemies by typing words correctly before they reach the player. As the game progresses, enemy difficulty increases, words become more complex, and players must balance both speed and accuracy to survive.

---

## Technologies
- Java 17
- Java Swing
- Java AWT
- Maven
- Jackson JSON
- JUnit 5
- TinySound Audio Library
- Object-Oriented Programming (OOP)
- Event-Driven Programming
- JSON Data Persistence
- Software Testing
- Javadoc Documentation
- Modular Software Architecture
- Git & GitHub

---

# Project Overview
Staying Alive was designed as an educational typing game that combines gameplay mechanics with player progression, account management, statistical tracking, and customizable game systems.

The application consists of multiple subsystems including:
- User Authentication
- Gameplay Engine
- Enemy Management
- Statistics Tracking
- Progression System
- Audio System
- Store and Currency System
- Power-Up System
- Cosmetic System
- Tutorial System
- Parental Controls
- Persistent Save Files

---

# My Contributions
My primary focus throughout the project was on:

## User Interface Development
Designed and implemented major portions of the Java Swing frontend including:
- Main Menu
- Login Screen
- Player Hub
- Gameplay UI
- Statistics Screen
- Tutorial System
- Screen Navigation Framework
- Keyboard Shortcut Support
- Window Management Utilities

### Skills Demonstrated
- Java Swing Development
- GUI Design
- Event-Driven Programming
- Navigation Systems
- User Experience Design
- Custom Component Rendering
- Keyboard Input Handling

---

## Documentation
Extensively documented project classes and methods using Javadoc.

### Skills Demonstrated
- Technical Documentation
- API Documentation
- Code Maintainability
- Software Engineering Standards

---

## Testing
Created and maintained JUnit test suites covering gameplay systems, account management, progression systems, statistics tracking, and enemy logic.

### Skills Demonstrated
- Unit Testing
- Integration Testing
- Validation Testing
- Software Quality Assurance
- Test-Driven Thinking

---

# Gameplay System
The core of Staying Alive revolves around typing-based combat.

## Features
- Real-time typing gameplay
- Dynamic enemy spawning
- Enemy movement and collision detection
- Focus-based targeting system
- Word-completion combat mechanics
- Player health system
- Score system
- Difficulty scaling
- Progressive level unlocking
- Performance tracking

### Skills Demonstrated
- Game Loop Design
- Real-Time Systems
- Collision Detection
- Event Processing
- State Management
- Gameplay Balancing

### Core Classes
- `Gameplay.java`
- `Enemy.java`
- `Enemy_Attribute.java`
- `LevelData.java`
- `LevelSelector.java`
- `Difficulty.java`

---

# Enemy System
Enemies advance toward the player and must be defeated by typing assigned words.

## Enemy Types
### Normal Enemy
- Basic enemy
- Single-word defeat condition

### Heart Enemy
- Multiple-word completion
- Increased rewards

### Big Enemy
- Greater durability
- Increased damage

### Boss Enemy
- Highest difficulty
- Highest rewards
- Multi-stage encounters

### Skills Demonstrated
- Object-Oriented Design
- Game Entity Systems
- Enumeration Usage
- Difficulty Balancing

### Core Classes
- `Enemy.java`
- `Enemy_Attribute.java`

---

# Account Management System
The game implements a persistent player-account system.

## Features
- Account creation
- Login authentication
- Password management
- Progress tracking
- Persistent save storage
- Coin management
- Avatar support

### Skills Demonstrated
- Authentication Systems
- Data Persistence
- User Management
- JSON Serialization

### Core Classes
- `Account.java`
- `AccountManagement.java`
- `Parental.java`
- `PlayerProgress.java`

---

# Statistics and Progression System
Player performance is tracked and saved between sessions.

## Statistics Tracked
- High Score
- Average WPM
- Peak WPM
- Accuracy
- Mistakes
- Attempts
- Play Time
- Current Level
- Completion Status

### Skills Demonstrated
- Performance Tracking
- Data Analytics
- Persistent User Data
- Progression Design

### Core Classes
- `LevelStatistic.java`
- `PlayerProgress.java`
- `StatsScreen.java`

---

# User Interface System
The project uses a custom Java Swing screen framework.

## Screens Implemented
### Main Menu
- Login access
- Tutorial access
- Parental controls access

### Login Screen
- User authentication
- Error handling
- Keyboard shortcuts

### Player Hub
- New Game
- Continue Game
- Store access
- Statistics access
- Tutorial access

### Gameplay Screen
- Real-time rendering
- Score tracking
- Health display
- Enemy rendering

### Statistics Screen
- Gameplay metrics
- Progress tracking
- Avatar display

### Tutorial Screen
- Multi-page onboarding system
- Keyboard navigation
- Progress indicators

### Game Store
- Power-up purchases
- Cosmetic purchases
- Coin tracking

### Parental Controls
- Account administration
- Password resets
- Statistics resets
- User creation

### Skills Demonstrated
- Java Swing
- Screen Architecture
- Event Handling
- UI Design
- Navigation Systems

### Core Classes
- `NavigationControl.java`
- `Screen.java`
- `MainMenuScreen.java`
- `LoginScreen.java`
- `PlayerScreen.java`
- `GameplayScreen.java`
- `GamePanel.java`
- `StatsScreen.java`
- `TutorialScreen.java`
- `GameStoreScreen.java`
- `ParentalControls.java`
- `WindowUtils.java`

---

# Power-Up System
Players can purchase and use special gameplay abilities.

## Available Power-Ups
### Time Stop
- Temporarily freezes enemies

### Area of Effect
- Damages nearby enemies

### Shield
- Blocks incoming damage

### Features
- Purchasing
- Equipping
- Activation
- Cooldown management

### Skills Demonstrated
- Interface Design
- Gameplay Mechanics
- State Management

### Core Classes
- `Powerup.java`
- `Power_type.java`
- `StoreItem.java`

---

# Cosmetic System
Players can customize their appearance using cosmetic items.

## Features
- Avatar customization
- Cosmetic purchases
- Inventory management

### Cosmetic Categories
- Hats
- Outfits

### Skills Demonstrated
- Customization Systems
- Inventory Design
- Object-Oriented Programming

### Core Classes
- `Cosmetic.java`
- `CosmeticType.java`

---

# Audio System
Sound effects are managed through TinySound.

## Audio Events
- Button clicks
- Enemy hits
- Player damage
- Typing errors
- Healing
- Power-up usage
- Level completion
- Game over

### Skills Demonstrated
- Third-Party Library Integration
- Event-Based Audio Systems

### Core Classes
- `AudioManager.java`

---

# Persistent Data Storage
Player information is stored locally using JSON files.

## Stored Information
### players.json
Stores:
- User accounts
- Passwords
- Coins
- Statistics
- Player progress

### master.json
Stores:
- Master password for parental controls

### Skills Demonstrated
- JSON Serialization
- Data Modeling
- File Persistence

---

# Testing
Automated testing was implemented using JUnit 5.

## Test Coverage
### Account Systems
- Account creation
- Statistics updates
- Progress management
- Password handling

### Gameplay Systems
- Scoring
- Lives
- Difficulty multipliers
- Level completion
- Game over conditions

### Enemy Systems
- Enemy attributes
- Defeat mechanics

### Progression Systems
- Level statistics
- Player progression

### Test Classes
- `AccountTest.java`
- `GameplayTest.java`
- `EnemyTest.java`
- `LevelStatisticTest.java`
- `PlayerProgressTest.java`

### Skills Demonstrated
- Unit Testing
- Integration Testing
- Software Validation
- Automated Testing

---

# Package Structure
```text
src/
├── accounts/
├── audio/
├── cosmetics/
├── game/
│   ├── enemies/
│   └── levels/
├── powerups/
├── sprites/
├── ui/
├── stats/
├── storage/
└── util/

test/
├── AccountTest.java
├── GameplayTest.java
├── EnemyTest.java
├── LevelStatisticTest.java
└── PlayerProgressTest.java

data/
├── players.json
└── master.json

docs/
└── ARCHITECTURE.md
```

---

# Key Learning Outcomes
Throughout this project I gained experience with:
- Software Engineering Practices
- Object-Oriented Design
- Java Swing Development
- Event-Driven Programming
- GUI Architecture
- User Authentication Systems
- JSON Persistence
- Data Serialization
- Gameplay Architecture
- Unit Testing
- Integration Testing
- Javadoc Documentation
- Team-Based Development
- Maven Build Systems
- Third-Party Library Integration
- Software Debugging
- Technical Documentation

---

# Future Improvements
Potential future enhancements include:
- Additional enemy types
- More levels and worlds
- Expanded cosmetic inventory
- Achievement system
- Leaderboards
- Additional power-ups
- Multiplayer support
- Cloud save functionality
- Enhanced animations
- Improved visual effects
- Expanded testing coverage
- Additional statistics and analytics

---

# Team Members
Developed as **Group 54** for COMPSCI 2212.
- Omar Soliman
- Osman Idris
- Mohamed Ahmed
- Malik Alghneimin
- Fardin Abbassi

---

# Portfolio Summary

Developed a Java-based typing game using Java Swing, Maven, Jackson JSON, TinySound, and JUnit 5. 
Contributed primarily to UI development, navigation systems, screen architecture, technical documentation, and automated testing. 
Implemented and documented multiple user-facing screens, keyboard navigation systems, Javadoc documentation standards, and validation tests while collaborating within a modular software engineering codebase.
