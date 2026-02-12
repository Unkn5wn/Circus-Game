# 🎪 Circus Animal Catching Game

A fun, circus-themed arcade game where you control a clown to catch falling circus animals for points! Built with pure HTML5, CSS, and JavaScript - no dependencies required!

## 🎮 Game Overview

Control a clown (🤡) as you catch various circus animals falling from the sky. Each animal is worth different points, and you have 60 seconds to catch as many as possible. Watch out for the gorilla though - it costs you points!

## ✨ Features

- 🎪 **10 Different Circus Animals** - Each with unique point values and spawn rates
- ⏱️ **60-Second Gameplay** - Fast-paced arcade action
- 🏆 **Top 5 Leaderboard** - Save your high scores with persistent storage
- 🎵 **Auto-Generated Circus Music** - Dynamic background music using Web Audio API
- 🔊 **Sound Effects** - Different sounds for each type of catch
- 🎮 **Dual Control Support** - Play with keyboard or Nintendo Switch controller (USB)
- 💾 **Data Persistence** - Scores and settings saved via localStorage
- 🎨 **Beautiful UI** - Glass morphism design with animated backgrounds
- 📱 **Responsive Design** - Works on various screen sizes
- ♿ **Accessible** - Full keyboard navigation support

## 🎯 How to Play

1. **Start the Game** - Select "Start Game" from the main menu
2. **Move the Clown** - Use arrow keys or controller to move in all directions
3. **Catch Animals** - Position the clown to catch falling animals
4. **Score Points** - Different animals are worth different points
5. **Avoid the Gorilla** - The gorilla (🦍) costs you 5 points!
6. **Beat the Clock** - You have 60 seconds to score as high as possible
7. **Save Your Score** - Enter your name and save to the leaderboard

## 🎮 Controls

### Keyboard Controls

| Action | In Game | In Menus |
|--------|---------|----------|
| **Move** | Arrow Keys | - |
| **Navigate Up/Down** | - | Arrow Up/Down or W/S |
| **Adjust Volume** | - | Arrow Left/Right |
| **Select/Confirm** | - | Enter or Space |
| **Back/Exit** | ESC | ESC |

### Nintendo Switch Controller (USB)

| Action | In Game | In Menus |
|--------|---------|----------|
| **Move** | Left Analog Stick | - |
| **Navigate** | - | Left Stick (Y-axis) or D-Pad |
| **Adjust Volume** | - | Left Stick (X-axis) |
| **Select/Confirm** | - | A Button |
| **Back/Exit** | B Button | B Button |

**Note:** Controller must be connected via USB for detection.

## 🐘 Animals & Points

| Animal | Emoji | Points | Spawn Weight | Rarity |
|--------|-------|--------|--------------|--------|
| **Rabbit** | 🐰 | **+50** | 2 | ⭐⭐⭐⭐⭐ Ultra Rare |
| **Bear** | 🐻 | **+25** | 5 | ⭐⭐⭐⭐ Rare |
| **Leopard** | 🐆 | **+20** | 6 | ⭐⭐⭐ Uncommon |
| **Tiger** | 🐯 | **+15** | 8 | ⭐⭐⭐ Uncommon |
| **Lion** | 🦁 | **+10** | 10 | ⭐⭐ Common |
| **Camel** | 🐪 | **+3** | 12 | ⭐ Very Common |
| **Zebra** | 🦓 | **+2** | 12 | ⭐ Very Common |
| **Monkey** | 🐵 | **+1** | 15 | ⭐ Very Common |
| **Elephant** | 🐘 | **+1** | 15 | ⭐ Very Common |
| **Gorilla** | 🦍 | **-5** ⚠️ | 8 | ⭐⭐ Common (AVOID!) |

### Strategy Tips:
- 🐰 **Rabbits are rare but worth 50 points** - prioritize them when they appear!
- 🦍 **Gorillas subtract 5 points** - avoid catching them if possible
- 🐻 **Bears are a great balance** - worth 25 points and appear occasionally
- 🐆 **Big cats (Leopard, Tiger, Lion)** - solid mid-range points
- The weighted spawn system means common animals appear much more frequently

## 🚀 Installation

No installation or build process required! Simply:

1. **Download or clone this repository**
   ```bash
   git clone https://github.com/Unkn5wn/Circus-Game.git
   cd Circus-Game
   ```

2. **Open `index.html` in any modern web browser**
   - Double-click the file, or
   - Right-click → Open with → Your browser
   - Or drag and drop into browser window

3. **Start playing immediately!**

### Requirements:
- Any modern web browser (Chrome, Firefox, Safari, Edge)
- JavaScript enabled
- No internet connection required after download

## 🛠️ Technologies Used

- **HTML5** - Structure and Canvas API for game rendering
- **CSS3** - Glass morphism effects, animations, responsive design
- **JavaScript (ES6+)** - Game logic and interactivity
- **Web Audio API** - Dynamic music generation and sound effects
- **Gamepad API** - Nintendo Switch controller support
- **LocalStorage API** - Persistent data storage for scores and settings
- **RequestAnimationFrame** - Smooth 60 FPS game loop

## 🎨 Game Screens

The game includes multiple screens for a complete experience:

1. **Main Menu** - Navigate to game, leaderboard, options, or credits
2. **Game Screen** - The main gameplay with HUD elements
3. **Game Over** - Score display with name input and save options
4. **Leaderboard** - Top 5 high scores with medals
5. **Options Menu** - Access to volume and controller settings
6. **Volume Control** - Separate controls for music and sound effects
7. **Controller Selection** - Choose between keyboard or Switch controller

## 🎵 Audio Features

### Background Music
- Procedurally generated using Web Audio API
- Triangle wave oscillator with melodic loop
- 8-note sequence in a cheerful circus theme
- Adjustable volume (0-100%)
- Starts automatically after first user interaction

### Sound Effects
- **Menu Click** - Satisfying click sound for navigation
- **Catch Sounds** - Different tones based on animal points:
  - High pitched celebration for rare animals (Rabbit)
  - Pleasant tones for valuable catches
  - Warning tone for the Gorilla
- Adjustable volume (0-100%)

## 💾 Data Persistence

All game data is stored locally in your browser:

### Leaderboard
- Stores top 5 high scores
- Includes player name and score
- Automatically sorts by score (highest first)
- Pre-populated with default scores on first run

### Settings
- Music volume preference
- Sound effects volume preference
- Controller type selection
- All settings persist across browser sessions

### Data Storage
- Uses browser's `localStorage`
- No server required
- No personal data collected
- Clear browser data to reset

## 📸 Screenshots

*Coming soon! Screenshots will be added to showcase:*
- Main menu with animated background
- Gameplay with falling animals
- Leaderboard with top scores
- Options and settings screens

## 🎮 Game Mechanics

### Physics
- **Player Speed:** 5 pixels per frame
- **Animal Fall Speed:** 2-4 pixels per frame (randomized)
- **Spawn Rate:** New animal every 1.5 seconds
- **Collision Detection:** Axis-Aligned Bounding Box (AABB)

### Canvas Details
- **Resolution:** 800x600 pixels
- **Background:** Multi-layer scene with sky, ground, buildings, circus tent, and trees
- **Rendering:** RequestAnimationFrame for smooth 60 FPS

### Weighted Spawn System
Animals spawn based on their weight value. Higher weight = more frequent spawning. This makes rare animals (like the Rabbit) appear much less often than common ones.

## 🐛 Known Behaviors

- **AudioContext Warning:** You may see a console warning about AudioContext. This is normal and harmless - it's a browser security feature. Music will start after your first interaction (button click).
- **Controller Detection:** For best results, connect your Nintendo Switch controller via USB before loading the page.
- **Audio on Mobile:** Some mobile browsers require a user gesture before playing audio. Tap any button to start the music.

## 🤝 Contributing

This is a complete single-file game, but suggestions and improvements are welcome! Feel free to:
- Fork the repository
- Create feature branches
- Submit pull requests
- Report issues or bugs

## 📝 License

MIT License

Copyright (c) 2024 Unkn5wn

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## 👨‍💻 Credits

**Created with ❤️ by Unkn5wn**

Special thanks to:
- Web Audio API for enabling procedural music generation
- The emoji creators for the fantastic animal characters
- You, for playing the game!

## 🎪 Enjoy the Game!

Have fun catching those circus animals! Try to beat the high score and see if you can catch the elusive rabbit! 🐰

---

*If you enjoy this game, please star the repository and share it with your friends!* ⭐
