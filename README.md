# 🐍 Python Snake Game

A classic Snake Game implementation using Python's Turtle graphics library. Control the snake, eat food, grow longer, and avoid hitting walls or yourself!

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Turtle](https://img.shields.io/badge/Graphics-Turtle-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## 🎮 Game Preview

```
┌─────────────────────────────────┐
│                                 │
│         ●  ← Food               │
│                                 │
│                                 │
│         ▓▓▓▓▓  ← Snake          │
│                                 │
│                                 │
│         Score: 5                │
│                                 │
└─────────────────────────────────┘
```

## ✨ Features

- **Classic Gameplay**: Control the snake with arrow keys
- **Score Tracking**: Keep track of your points
- **Collision Detection**: Game ends when hitting walls or yourself
- **Smooth Animation**: Optimized screen refresh rate
- **Growing Mechanism**: Snake extends when eating food
- **Food Respawn**: Random food placement after consumption

## 🎯 Game Rules

1. Use **arrow keys** to control the snake's direction
2. Eat the **blue food** to grow longer and increase your score
3. Avoid hitting the **walls**
4. Avoid hitting **your own tail**
5. Each food eaten = **+1 point**

## 🚀 Installation

### Prerequisites
- Python 3.8 or higher
- Turtle graphics library (comes pre-installed with Python)

### Setup

```bash
# Clone the repository
git clone https://github.com/Tariq728/snake-game.git

# Navigate to project directory
cd snake-game

# Run the game
python main.py
```

## 📁 Project Structure

```
snake-game/
│
├── main.py           # Main game loop and logic
├── snake.py          # Snake class (movement, growth)
├── food.py           # Food class (positioning, respawn)
├── scoreboard.py     # ScoreBoard class (scoring, game over)
├── README.md         # Project documentation
└── requirements.txt  # Dependencies (if any)
```

## 🎮 Controls

| Key | Action |
|-----|--------|
| ⬆️ Up Arrow | Move Up |
| ⬇️ Down Arrow | Move Down |
| ⬅️ Left Arrow | Move Left |
| ➡️ Right Arrow | Move Right |

## 🔧 Configuration

You can customize the game by modifying these parameters in `main.py`:

```python
# Screen dimensions
screen.setup(width=600, height=600)

# Game speed (lower = faster)
time.sleep(0.1)

# Collision detection distance
if snake.head.distance(food) < 15:  # Food collision
if snake.head.distance(segment) < 10:  # Self collision
```

## 📝 Code Structure

### main.py
- Initializes game screen and components
- Handles game loop and collision detection
- Manages keyboard input

### snake.py
- `Snake` class: Creates and manages snake segments
- `move()`: Moves snake forward
- `up()`, `down()`, `left()`, `right()`: Direction controls
- `extend()`: Adds new segment when eating food

### food.py
- `Food` class: Creates food object
- `refresh()`: Repositions food randomly

### scoreboard.py
- `ScoreBoard` class: Displays current score
- `count_score()`: Increments score
- `game_over()`: Displays game over message

## 🎨 Customization Ideas

Want to make it your own? Try these modifications:

1. **Add Difficulty Levels**: Increase speed as score increases
2. **Power-ups**: Add special food types with bonuses
3. **Obstacles**: Add stationary barriers
4. **High Score**: Save and display best score
5. **Sound Effects**: Add audio for eating and game over
6. **Color Themes**: Customize snake and background colors

## 🐛 Known Issues

- None currently reported

## 🔮 Future Enhancements

- [ ] Add pause functionality
- [ ] Implement high score persistence
- [ ] Add difficulty levels
- [ ] Create start menu
- [ ] Add sound effects
- [ ] Implement multiplayer mode
- [ ] Add power-ups and obstacles

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

**Tariq Anwar**
- GitHub: [@Tariq728](https://github.com/Tariq728)
- LinkedIn: [Tariq Anwar](https://www.linkedin.com/in/tariqanwar2000)
- Email: tariqanwar917@gmail.com

## 🙏 Acknowledgments

- Built as part of Python learning journey
- Inspired by the classic Nokia Snake game
- Thanks to the Python Turtle graphics library

## 📸 Screenshots

*Add screenshots of your game here after uploading*

---

**Enjoy the game! 🎮🐍**

*If you found this project helpful, please consider giving it a ⭐ on GitHub!*
