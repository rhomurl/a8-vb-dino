# 🦕 Dino Runner - Ancient8 Edition

A modern, feature-rich remake of the classic Chrome dinosaur game with exciting gameplay mechanics, multiple characters, power-ups, and dynamic themes. Perfect for players from kids to GenZ!

![Game Preview](https://via.placeholder.com/800x400?text=Dino+Runner+Game+Preview)

## 🎮 Features

### 🦖 Multiple Characters
Choose from 6 unique unlockable characters:
- **🦕 Dino** - The classic runner
- **🐍 Snake** - Slithers with S-shaped movement
- **🐶 Dog** - Runs with animated legs and floppy ears
- **🐱 Cat** - Agile with pointed ears and green eyes
- **🐅 Tiger** - Fierce with black stripes
- **🕷️ Spider** - Creepy crawler with 8 animated legs

### 🌈 Universal Color System
All characters support 9 color variations:
- **Classic** Gray (Free)
- **Red** (1 coin)
- **Blue** (2 coins)
- **Green** (3 coins)
- **Orange** (4 coins)
- **Purple** (5 coins)
- **Teal** (6 coins)
- **Dark** (7 coins)
- **Rainbow** ✨ (10 coins) - Animated rainbow effect!

### ⚡ Power-Up System
Collect power-ups for special abilities:
- **🚀 Speed Boost** - Increases movement speed and score multiplier
- **⭐ Invincibility** - Temporary immunity to obstacles with golden glow
- **⬆️ Double Jump** - Extra jump to reach higher birds

### 🪙 Economy & Progression
- **Coin Collection** - Gather coins to unlock new content
- **Combo System** - Chain collections for score multipliers
- **Shop System** - Spend coins on characters and colors
- **Achievement Milestones** - Celebration animations at score landmarks

### 🌍 Dynamic Themes
Background automatically changes every 250 points:
1. **Day** - Bright sky with white clouds
2. **Sunset** - Orange and yellow gradient
3. **Night** - Dark sky with twinkling stars
4. **Space** - Deep purple cosmos with stars
5. **Ocean** - Blue underwater with floating bubbles

### 💥 Visual Effects
- **Screen Shake** - Impact feedback for jumps and collisions
- **Particle Systems** - Explosion effects and landing dust
- **Animated Elements** - Moving clouds, character animations
- **Power-up Glow** - Visual feedback for active abilities

## 🎯 Controls

### Desktop
- **Jump**: `SPACEBAR` or `↑ Arrow`
- **Crouch**: `↓ Arrow` 
- **Double Jump**: Jump again while airborne (with power-up)
- **Pause**: `P` key
- **Restart**: `R` key
- **Shop**: `S` key

### Mobile/Touch
- **Jump**: Tap screen
- **Crouch**: Swipe down
- **Double Jump**: Tap again while jumping

## 🏆 Gameplay Mechanics

### Jump System
- **Regular Jump**: Clears cacti obstacles (-12 velocity)
- **Double Jump**: Higher jump to clear birds (-10 velocity)
- **Canvas Bounds**: Jumps stay within visible area

### Obstacle Types
- **🌵 Cacti**: Ground-level obstacles (jump to avoid)
- **🐦 Birds**: Flying obstacles at 60px height (double jump to clear)

### Scoring System
- **Base Score**: 10 points per second
- **Speed Multiplier**: 1.5x during speed boost
- **Combo Bonus**: Extra points for consecutive coin collection
- **Milestone Rewards**: Special celebrations every 500 points

### Difficulty Progression
- **Speed Increase**: Game gradually speeds up over time
- **Dynamic Spawning**: Obstacle frequency scales with current speed
- **Theme Progression**: Visual variety every 250 points

## 🛒 Shop System

### Character Prices
- 🦕 Dino: **Free**
- 🐍 Snake: **3 coins**
- 🐶 Dog: **4 coins**
- 🐱 Cat: **5 coins**
- 🐅 Tiger: **8 coins**
- 🕷️ Spider: **10 coins**

### Color Prices
- Classic: **Free**
- Basic Colors: **1-7 coins**
- Rainbow: **10 coins**

*Demo-friendly pricing for easy testing!*

## 🚀 Getting Started

1. **Open the Game**: Open `index.html` in any modern web browser
2. **Start Playing**: Press spacebar or click to jump
3. **Collect Coins**: Grab golden coins for shop purchases
4. **Get Power-ups**: Lightning bolts, stars, and arrows
5. **Visit Shop**: Press 'S' to unlock characters and colors
6. **Enjoy Themes**: Watch backgrounds change every 250 points!

## 🔧 Technical Details

### Architecture
- **Single HTML File**: All code contained in `index.html`
- **Canvas-based Rendering**: HTML5 Canvas API for smooth graphics
- **Local Storage**: Saves coins, unlocks, and high scores
- **60fps Game Loop**: requestAnimationFrame for smooth gameplay

### Performance
- **Optimized Rendering**: Efficient particle and animation systems
- **Memory Management**: Automatic cleanup of off-screen objects
- **Responsive Design**: Works on desktop and mobile devices

### Browser Support
- Modern browsers with HTML5 Canvas support
- Chrome, Firefox, Safari, Edge
- Mobile browsers on iOS and Android
- Graceful fallback for older browsers

### Error Handling & Stability
- **Canvas Detection**: Automatic fallback for unsupported browsers
- **Safe localStorage**: Corrupted save data recovery with defaults
- **Bounds Checking**: Prevents character from jumping outside canvas
- **Performance Limits**: Particle systems capped to prevent lag
- **Error Recovery**: Game loop error handling prevents crashes

## 📊 Game Statistics Tracking

The game automatically tracks and saves:
- **High Score**: Best score achieved
- **Total Coins**: Coins earned across all games
- **Max Combo**: Highest combo chain achieved
- **Unlocked Characters**: Purchased characters persist
- **Unlocked Colors**: Purchased colors persist
- **Current Selections**: Active character and color

## 🎨 Customization

### Adding New Characters
1. Add character data to `characterData` array
2. Create drawing function in `drawCharacter()` switch
3. Implement color support using `getSkinColors()`

### Adding New Themes
1. Add theme to `getThemes()` function
2. Define colors and special elements
3. Add theme-specific drawing in `drawThemeElements()`

### Adding New Power-ups
1. Add power-up type to spawn system
2. Create collection logic in `collectPowerUp()`
3. Implement effects in character update functions

## 📈 Score Breakdown

### Base Scoring
- **Survival**: 10 points/second
- **Obstacle Avoidance**: 10 points per obstacle passed
- **Coin Collection**: 10 points per coin + combo bonus

### Multipliers
- **Speed Boost**: 1.5x score multiplier
- **Combo System**: 1 + (combo × 0.1) multiplier
- **Milestone Bonuses**: Special score events

## 🎉 Achievement System

### Milestone Celebrations
- **500 points**: "Great job!" 🎉
- **1000 points**: "Amazing!" 🚀
- **2000 points**: "On fire!" 🔥
- **3000 points**: "Superstar!" ⭐
- **5000 points**: "Champion!" 🏆
- **7500 points**: "Mind blown!" 🤯
- **10000 points**: "Legendary!" 👑

## ✅ Quality Assurance

### Bug Fixes Applied
- **localStorage Safety**: Added try-catch for corrupted save data
- **Canvas Bounds**: Characters can't jump above visible area
- **Performance**: Limited particles to prevent lag spikes
- **Error Handling**: Graceful degradation for unsupported features
- **Shop Layout**: Responsive grid system for different screen sizes
- **Game Loop**: Protected against infinite loops and crashes

## 🐛 Known Limitations

- No sound effects (browser-based, no audio files)
- Single-player only
- No online leaderboards
- Limited to preset themes and characters

## 🔮 Future Enhancements

Potential features for future versions:
- Sound effects and background music
- Additional characters and themes
- Multiplayer racing mode
- Online leaderboards
- Level editor
- Power-up combinations

## 📜 License

This project is a fan-made recreation inspired by the classic Chrome dinosaur game. Built for educational and entertainment purposes.

---

**Have fun running and jumping! 🦕💨**

*Created with ❤️ using HTML5, CSS3, and vanilla JavaScript*