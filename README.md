# 🏓 Bouncing Ball Game

A classic arcade-style bouncing ball game built with HTML5 Canvas and JavaScript. Control the paddle to keep the ball bouncing and prevent it from hitting the bottom of the screen!


##  Game Overview

This is a simple yet engaging bouncing ball game where players use a paddle to keep a red ball bouncing within the game area. The objective is to prevent the ball from falling off the bottom of the screen by moving the paddle left and right to hit the ball back up.

### ✨ Features

- **Smooth Animation**: Fluid ball movement and paddle controls using `requestAnimationFrame`
- **Collision Detection**: Physics-based collision detection for walls and paddle interactions
- **Responsive Controls**: Arrow key controls for paddle movement
- **Game State Management**: Start, restart, and game over functionality
- **Modern UI**: Clean, modern design with rounded corners and shadows
- **Object-Oriented Code**: Well-structured code using ES6 classes

## Preview

- [Play the game](https://haseebjaved4212.github.io/Bouncing-Ball-Game/)


##  Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- No additional installations required!

### Installation & Setup

1. **Clone or Download** the project files to your local machine
2. **Navigate** to the project directory
3. **Open** `index.html` in your web browser



### Running the Game

1. Open `index.html` in your web browser
2. Click the **"Start Game"** button
3. Use the **Left** and **Right** arrow keys to control the paddle
4. Keep the ball bouncing by hitting it with the paddle
5. If the ball hits the bottom, the game ends - click **"Restart Game"** to play again

##  How to Play

### Controls

- **Left Arrow Key** (←): Move paddle left
- **Right Arrow Key** (→): Move paddle right
- **Start Game Button**: Begin a new game or restart after game over

### Objective

- Keep the ball bouncing by hitting it with your paddle
- The ball bounces off the walls (left, right, and top)
- Don't let the ball fall off the bottom of the screen!
- If the ball hits the bottom without touching the paddle, it's game over

### Game Mechanics

- The ball starts in the center-bottom area moving upward
- Ball speed is constant throughout the game
- Paddle movement speed is responsive and smooth
- Collision detection ensures realistic physics behavior

## Technical Details

### File Structure

```
Bouncing Ball Game/
├── index.html        # Main HTML file with game setup
├── style.css          game layout and styling
├── script.js           # Game logic and JavaScript functionality
└── README.md           # This documentation file
```

### Architecture

#### **HTML Structure** (`index.html`)

- Responsive layout with centered game container
- HTML5 Canvas element for game rendering
- Control buttons and message display area
- Modern CSS styling with Inter font family

#### **JavaScript Classes** (`script.js`)

- **`Ball` Class**: Manages ball properties, movement, and rendering
  - Properties: position (x, y), velocity (dx, dy), radius
  - Methods: `draw()`, `update()`
- **`Paddle` Class**: Handles paddle rendering and properties
  - Properties: position (x), dimensions (width, height)
  - Methods: `draw()`

#### **Game Functions**

- `gameLoop()`: Main game loop using requestAnimationFrame
- `checkCollisions()`: Handles wall and paddle collision detection
- `updatePaddlePosition()`: Processes keyboard input for paddle movement
- `startGame()`: Initializes game state and starts the game loop
- `handleGameOver()`: Manages game over state and UI updates

### Key Technologies

- **HTML5 Canvas**: For 2D graphics rendering
- **JavaScript ES6**: Modern JavaScript with classes and arrow functions
- **CSS3**: Modern styling with flexbox, transitions, and box shadows
- **RequestAnimationFrame**: For smooth 60fps game animation

##  Customization

### Modifying Game Parameters

You can easily customize various aspects of the game by editing `script.js`:

```javascript
// Ball properties (in Ball class constructor)
this.radius = 10; // Ball size
this.dx = 2; // Horizontal speed
this.dy = -2; // Vertical speed

// Paddle properties (in Paddle class constructor)
this.height = 10; // Paddle thickness
this.width = 75; // Paddle width

// Paddle movement speed (in updatePaddlePosition function)
const paddleSpeed = 7; // How fast paddle moves
```

### Styling Changes

Modify the CSS in `index.html` to change:

- Colors (ball, paddle, background)
- Canvas size
- Button styling
- Typography and layout

### Adding Features

Consider implementing these enhancements:

- Score tracking
- Multiple balls
- Power-ups
- Increasing difficulty
- Sound effects
- Particle effects

##  Troubleshooting

### Common Issues

**Game doesn't start:**

- Ensure JavaScript is enabled in your browser
- Check browser console for any error messages

**Paddle doesn't move:**

- Make sure the game canvas has focus (click on it)
- Verify arrow keys are not being intercepted by browser

**Performance issues:**

- Close other browser tabs
- Try a different browser
- Check if hardware acceleration is enabled

##  Contributing

This is a simple educational project, but contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch
3. Make your improvements
4. Submit a pull request

### Ideas for Contributions

- Add sound effects
- Implement scoring system
- Create multiple difficulty levels
- Add mobile touch controls
- Include game statistics

##  License

This project is open source available for use and modification.

##  Acknowledgments

- Built with vanilla JavaScript for educational purposes
- Inspired by classic arcade games like Pong and Breakout
- Uses modern web technologies for smooth gameplay

---

**Enjoy playing the Bouncing Ball Game!**

For questions or suggestions, feel free to open an issue or reach out!
