# Marrow

A turn-based card battle game built in Java using Swing. Fight against various enemies using attack and defense cards, upgrade your character, and see how long you can survive!

## Game Overview

Marrow is a strategic card-based combat game where you face increasingly difficult enemies using a deck of attack and defense cards. The game features:

- **Turn-based combat** - Choose between attack and defense cards each turn
- **Enemy progression** - Enemies become stronger with more HP, damage, and armor as you progress
- **Character upgrades** - Improve your health, defense, attack power, and shield effectiveness
- **Critical hits** - Both you and enemies can deal critical damage
- **Armor system** - Later enemies have armor that must be broken or penetrated
- **High score tracking** - Your best runs are saved to `highscore.txt`

### Combat Mechanics

- **Attack Cards**: Deal 3-5 base damage to enemies (can be upgraded)
- **Defense Cards**: Gain 2-4 defense points (can be upgraded) 
- **Critical Hits**: 1% chance for player, 20% chance for enemies
- **Enemy Scaling**: Every 2 enemies defeated increases enemy HP and adds armor
- **Armor Penetration**: Some armored enemies can penetrate through your defense

### Upgrade System

After defeating each enemy, choose from 4 upgrade types:
- **Health**: Increase maximum HP by 1
- **Defense**: Increase base defense by 1  
- **Attack**: Increase maximum attack damage by 0.5
- **Shield**: Increase defense card effectiveness by 0.5

## How to Run

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- Command line access (PowerShell, Command Prompt, or Terminal)

### Running the Game

1. **Clone the project and navigate to the game directory:**
   ```powershell
   cd "C:\Users\...\"
   ```

2. **Compile the Java files:**
   ```powershell
   javac *.java
   ```

3. **Run the game:**
   ```powershell
   java MarrowExecutable
   ```

### Alternative: Using an IDE
You can also open the project in any Java IDE (like IntelliJ IDEA, Eclipse, or VS Code with Java extensions) and run the `MarrowExecutable.java` file directly.

## Game Controls

- **Mouse**: Click on cards to use them
- **Window**: The game supports fullscreen mode and window resizing
- **Menu**: Use the "Start Game" button to begin, and you can return to menu after game over

## Project Structure

```
Marrow/
├── MarrowExecutable.java    # Main game launcher and window management
├── GameLogic.java          # Core game mechanics and state management
├── GamePanel.java          # Game interface and rendering
├── MenuPanel.java          # Main menu interface
├── DrawingArea.java        # Game drawing utilities
├── RetroPanel.java         # Additional UI components
├── highscore.txt          # High score storage
├── sprites/               # Game assets
│   ├── attack.png         # Attack card sprite
│   ├── defense.png        # Defense card sprite
│   ├── heart.png          # HP indicator
│   ├── HPCARD.png         # Health upgrade card
│   └── Enemies/           # Enemy sprites
└── LICENSE                # MIT License
```

## Features

- **Responsive UI**: Scales properly with window resizing and fullscreen mode
- **Visual Feedback**: Animated sprites and card effects
- **Persistent High Scores**: Your best runs are automatically saved
- **Balanced Gameplay**: Carefully tuned damage, defense, and upgrade systems
- **Multiple Enemy Types**: 10+ different enemy sprites with unique appearances

## Development

This is a Java Swing application following object-oriented design principles:
- **Singleton Pattern**: Used for GameLogic to maintain single game state
- **Observer Pattern**: Event-driven UI updates
- **MVC Architecture**: Separation of game logic, UI, and data

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Credits

Copyright (c) 2025 JA-Dilao

---

*Good luck surviving the depths! How many enemies can you defeat?*
