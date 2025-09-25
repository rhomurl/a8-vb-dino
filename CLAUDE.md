# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-file HTML5 canvas game - "Dino Runner - Ancient8 Edition" - a Chrome dinosaur game clone built entirely in vanilla JavaScript. The entire game is contained within `index.html` with embedded CSS and JavaScript.

## Architecture

### Game Structure
- **Single HTML file architecture**: All code (HTML, CSS, JS) is contained in `index.html`
- **Canvas-based rendering**: Uses HTML5 Canvas API for all game graphics
- **Game loop pattern**: Implements requestAnimationFrame-based game loop with delta time
- **State management**: Simple string-based game states ('playing', 'gameOver', 'paused')
- **Local storage**: High scores are persisted using localStorage

### Core Game Systems
- **Physics**: Custom gravity and collision detection system
- **Entity system**: Dino player character with obstacles (cacti and birds)
- **Particle system**: Visual effects for landing and interactions
- **Input handling**: Keyboard, mouse, and touch controls
- **Background elements**: Animated clouds and parallax effects

## Development Commands

Since this is a static HTML file, there are no build commands or package managers. Development workflow:

1. **Run the game**: Open `index.html` directly in a web browser
2. **Development**: Edit `index.html` directly - changes are immediately visible on browser refresh
3. **Testing**: Manual testing in browser (no automated test framework)

## Key Components

### Game Objects
- `dino`: Player character with jump/crouch mechanics
- `obstacles[]`: Array of cacti and birds that move toward player
- `particles[]`: Visual effect system
- `clouds[]`: Background decoration

### Game Logic (lines 180-604)
- Game loop with delta time management
- Collision detection using AABB (axis-aligned bounding box)
- Score system with speed scaling
- High score persistence

### Controls
- **Jump**: SPACEBAR, ↑ Arrow, Click/Tap
- **Crouch**: ↓ Arrow, Swipe Down
- **Pause**: P key
- **Restart**: R key

### Game Balance
- Speed increases over time (line 348)
- Dynamic obstacle spawning based on current speed (line 300)
- Score increases both over time and by avoiding obstacles

## Code Conventions

- Uses ES6+ JavaScript features
- Camel case for variables and functions
- Game constants and state stored in global scope
- Event-driven input handling
- Canvas 2D context for all rendering
- No external dependencies or frameworks