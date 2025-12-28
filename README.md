# YetAnotherHangmanGame

A beautiful, feature-rich Hangman game built with Python and PyQt5, featuring multiple word categories, customizable themes, and persistent score tracking.

![Python Version](https://img.shields.io/badge/python-3.6%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## Features

- 🎨 **8 Beautiful Themes** - Choose from Ocean Breeze, Sunset Glow, Cotton Candy, Forest Mist, Lavender Dream, Midnight Sky, Coral Reef, and Mint Fresh
- 📚 **Multiple Word Categories** - Animals, Aquatic creatures, Foods, Cities, and Countries
- ⌨️ **Dual Input Methods** - Click letter buttons or use your keyboard
- 📊 **Score Tracking** - Automatic wins/losses tracking with persistent storage
- 🎮 **Smooth Gameplay** - Instant feedback and smooth transitions
- 💾 **Auto-save** - Scores are automatically saved to your home directory

## Screenshots

The game features a clean, modern interface with customizable color themes and an intuitive layout.

## Requirements

- Python 3.6 or higher
- PyQt5

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Skatterbrainz/YetAnotherHangmanGame.git
   cd YetAnotherHangmanGame
   ```

2. **Install dependencies**
   ```bash
   pip install PyQt5
   ```

   Or using a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install PyQt5
   ```

## Usage

Run the game with:
```bash
python hangman.py
```

### How to Play

1. **Select a category** from the dropdown menu (Animals, Aquatic, Foods, Cities, or Countries)
2. **Choose a theme** to customize the game's appearance
3. **Guess letters** by clicking the on-screen buttons or pressing keys on your keyboard
4. **Win the game** by guessing all letters before the hangman is complete
5. **Track your progress** with the win/loss counter at the top

### Game Rules

- You have 7 incorrect guesses before losing
- Each incorrect guess adds a body part to the hangman
- Correctly guessed letters are revealed in the word
- Already guessed letters are disabled and shown in the "Tried" list

## Word Categories

- **Animals**: 33 words including elephant, giraffe, penguin, and more
- **Aquatic**: 12 words featuring ocean creatures like dolphin, shark, and octopus
- **Foods**: 15 delicious words from pizza to sukiyaki
- **Cities**: 32 cities from around the world
- **Countries**: 30+ countries across all continents

## Themes

Choose from 8 carefully crafted color themes:
- **Ocean Breeze** - Cool blues reminiscent of the sea
- **Sunset Glow** - Warm oranges and amber tones
- **Cotton Candy** - Sweet pinks and purples
- **Forest Mist** - Fresh, earthy greens
- **Lavender Dream** - Elegant purple hues
- **Midnight Sky** - Deep, rich blues
- **Coral Reef** - Vibrant coral and orange shades
- **Mint Fresh** - Refreshing teal and mint colors

## Score Storage

Your scores are automatically saved to `.hangman_scores.json` in your home directory and persist between game sessions.

## Development

### Project Structure
```
YetAnotherHangmanGame/
├── hangman.py          # Main game file
├── README.md           # This file
└── LICENSE             # License information
```

### Extending the Game

You can easily add more word categories by editing the `WORDS` dictionary in [hangman.py](hangman.py):

```python
WORDS = {
    "your_category": ["word1", "word2", "word3"],
    # ... existing categories
}
```

Or add new themes by extending the `THEMES` dictionary:

```python
THEMES = {
    "Your Theme": {
        "bg": "#FFFFFF",       # Background color
        "primary": "#000000",  # Primary button color
        "secondary": "#333333", # Secondary/hover color
        "text": "#000000"      # Text color
    },
    # ... existing themes
}
```

## Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Add more word categories
- Create new themes
- Improve documentation

Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

**Skatterbrainz**
- GitHub: [@Skatterbrainz](https://github.com/Skatterbrainz)

## Acknowledgments

- Built with PyQt5 for a modern, cross-platform GUI experience
- Inspired by the classic word-guessing game

## Version History

- **1.0** (2025-12-28) - Initial release
  - Multiple word categories
  - 8 customizable themes
  - Keyboard and mouse input
  - Persistent score tracking

---

Enjoy playing! 🎮
