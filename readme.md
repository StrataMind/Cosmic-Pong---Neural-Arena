# 🎮 Cosmic Pong - Neural Arena

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Canvas API](https://img.shields.io/badge/Canvas_API-FF6B35?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)

A modern, visually stunning take on the classic Pong game featuring AI opponents, multiple game modes, power-ups, and responsive design. Built with pure HTML5, CSS3, and JavaScript.

## 🌟 Features

- **🎯 Four Unique Game Modes** - Classic, Speed Rush, Survival, and Power Arena
- **🤖 Adaptive AI** - Neural AI that evolves and becomes more challenging
- **📱 Cross-Platform** - Responsive design works on desktop, tablet, and mobile
- **🎨 Modern UI/UX** - Glassmorphism design with particle effects and animations
- **🔊 Dynamic Audio** - Procedural sound generation with toggle controls
- **⚡ High Performance** - 60 FPS gameplay with optimized Canvas rendering
- **🎮 Multiple Controls** - Mouse, touch, and keyboard support

## 🕹️ Game Modes

### ⚡ Classic Mode
Traditional Pong experience with modern visuals. Race against time to score the most points.
- **Duration:** 1, 3, or 5 minutes
- **Features:** Pure pong gameplay, combo system

### 🚀 Speed Rush
Ball speed increases every 10 seconds, testing your reflexes as chaos ensues.
- **Speed Multiplier:** Up to 2.5x base speed
- **Escalation:** +0.3x speed every 10 seconds

### 🛡️ Survival
AI evolves every 30 seconds, becoming faster and smarter. How long can you survive?
- **AI Difficulty:** Scales up to 2.5x base difficulty
- **Evolution:** +0.4x AI skill every 30 seconds

### ⭐ Power Arena
Collect power-ups every 20 seconds to gain temporary advantages.
- **Power-ups:** Speed boost, paddle size increase
- **Duration:** 5-second power-up effects
- **Spawn Rate:** Every 20 seconds

## 🎮 Controls

| Control | Action |
|---------|--------|
| **Mouse Movement** | Control player paddle |
| **Touch/Swipe** | Mobile paddle control |
| **SPACE** | Pause/Resume game |
| **Sound Icon** | Toggle audio on/off |

## 🚀 Getting Started

### Prerequisites
- Modern web browser with HTML5 Canvas support
- JavaScript enabled
- Audio API support (optional, for sound effects)

### Installation

1. **Download the game file**
   ```bash
   # Clone if part of a repository
   git clone https://github.com/surajsk2003/cosmic-pong.git
   cd cosmic-pong
   ```

2. **Run locally**
   - Simply open `index.html` in your web browser
   - Or serve through a local server for best performance:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   ```

3. **Play online**
   - Open the hosted version directly in your browser

## 🏗️ Technical Architecture

### Core Components

```
CosmicPong Class
├── Game State Management
├── Canvas Rendering Engine
├── Physics & Collision System
├── AI Behavior System
├── Audio System
├── Input Handling
└── UI Management
```

### Key Technical Features

- **Canvas-based Rendering**: Smooth 60 FPS gameplay
- **Responsive Design**: Adapts to screen sizes from 320px to 1920px+
- **Performance Optimization**: Delta time normalization, frame limiting
- **Modern JavaScript**: ES6+ features, modular architecture
- **CSS3 Animations**: Hardware-accelerated transitions and effects

### File Structure

```
cosmic-pong/
├── index.html          # Main game file (self-contained)
├── README.md           # This documentation
└── assets/            # Optional assets directory
    ├── screenshots/   # Game screenshots
    └── demo/         # Demo videos or GIFs
```

## 🎨 Customization

### Modifying Game Parameters

The game is highly customizable. Key parameters you can adjust:

```javascript
// Paddle settings
paddleWidth: canvas.width * 0.008
paddleHeight: canvas.height * 0.12
paddleSpeed: 8

// Ball settings
ballRadius: canvas.width * 0.006
baseSpeed: canvas.width * 0.004

// Game modes
speedIncrease: 0.3  // Speed Rush mode
aiDifficultyIncrease: 0.4  // Survival mode
powerUpDuration: 5000  // Power Arena mode
```

### Adding New Game Modes

1. Add mode configuration in the `applyModeEffects()` method
2. Create UI elements in the mode selection screen
3. Implement mode-specific logic in the update loop

### Visual Customization

- **Colors**: Modify CSS custom properties
- **Particles**: Adjust particle count and behavior
- **UI Elements**: Customize glassmorphism effects and animations

## 🌐 Browser Support

| Browser | Minimum Version | Notes |
|---------|----------------|-------|
| **Chrome** | 60+ | Full support |
| **Firefox** | 55+ | Full support |
| **Safari** | 12+ | Full support |
| **Edge** | 79+ | Full support |
| **Mobile Safari** | 12+ | Touch controls |
| **Chrome Mobile** | 60+ | Touch controls |

### Required APIs
- HTML5 Canvas
- Web Audio API (optional)
- Touch Events (mobile)
- RequestAnimationFrame

## 📊 Performance

### Optimizations Implemented
- **Delta Time Normalization**: Consistent gameplay across frame rates
- **Object Pooling**: Efficient particle management
- **Canvas Optimization**: Minimal redraws, efficient rendering
- **Memory Management**: Proper cleanup of game objects

### Performance Metrics
- **Target FPS**: 60 FPS
- **Memory Usage**: ~10-20MB
- **CPU Usage**: ~5-15% on modern devices
- **Mobile Performance**: Optimized for 30+ FPS on mid-range devices

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Bug Reports
1. Check existing issues first
2. Provide detailed reproduction steps
3. Include browser/device information
4. Add screenshots if applicable

### Feature Requests
1. Describe the feature clearly
2. Explain the use case
3. Consider implementation complexity
4. Discuss with maintainers first

### Development Setup
```bash
# Fork the repository
git clone https://github.com/yourusername/cosmic-pong.git
cd cosmic-pong

# Create a feature branch
git checkout -b feature/your-feature-name

# Make your changes and test thoroughly
# Submit a pull request with detailed description
```

### Code Style Guidelines
- Use consistent indentation (2 spaces)
- Follow ES6+ standards
- Comment complex logic
- Maintain performance considerations

## 📈 Roadmap

### Planned Features
- [ ] Multiplayer support (local and online)
- [ ] Tournament mode with brackets
- [ ] Custom paddle and ball skins
- [ ] Advanced AI personalities
- [ ] Mobile app version
- [ ] Leaderboard system
- [ ] Replay system
- [ ] Advanced statistics

### Known Issues
- Audio may not work on some mobile browsers without user interaction
- Performance may vary on older devices
- Touch controls sensitivity varies by device

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2024 Suraj Singh

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
```

## 🙏 Acknowledgments

- Inspired by the classic Pong game by Atari
- Modern design influenced by glassmorphism trends
- Audio system inspired by procedural music generation
- Community feedback and testing

## 📞 Contact

**Suraj Singh**
- Portfolio: [surajsk2003.github.io/Suraj.in](https://surajsk2003.github.io/Suraj.in)
- GitHub: [@surajsk2003](https://github.com/surajsk2003)
- LinkedIn: [Suraj Singh](https://www.linkedin.com/in/suraj-singh-96b45220a)
- Email: surajkumarsksk2000@gmail.com

---

<div align="center">

**⭐ Star this repository if you enjoyed the game! ⭐**

[Play Now](https://surajsk2003.github.io/cosmic-pong) | [Report Bug](https://github.com/surajsk2003/cosmic-pong/issues) | [Request Feature](https://github.com/surajsk2003/cosmic-pong/issues)

</div>