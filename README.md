# Acronym Bingo

An interactive web-based quiz application to test your knowledge of acronyms across various professional domains including ICT, Data Engineering, Analytics, Security, Cloud Computing, and more.

## Features

- **15 Categories** spanning different professional domains
- **900+ Acronyms** to test your knowledge
- **10 Questions per Quiz** randomly selected from each category
- **Real-time Scoring** with instant feedback
- **Responsive Design** works on desktop, tablet, and mobile
- **Progress Tracking** visual progress bar throughout the quiz
- **Detailed Results** showing correct answers for review

## Categories

- 💻 ICT & Infrastructure
- 🗄️ Data Engineering
- 📊 Analytics & BI
- 💼 Consulting
- 🎖️ Military
- ☁️ Cloud & DevOps
- 🔒 Security & Compliance
- 💾 Databases
- 🤖 AI & Machine Learning
- ⚙️ Software Development
- 💰 Finance & Accounting
- 👥 Human Resources
- 📱 Marketing & Sales
- 📡 Telecommunications
- 🏥 Healthcare & Medical

## Demo

Visit the live demo: [https://Xudo-Data-Boutique.github.io/acronym-bingo](https://Xudo-Data-Boutique.github.io/acronym-bingo)

## Installation

### Option 1: GitHub Pages (Recommended)

1. Fork this repository
2. Go to repository Settings → Pages
3. Under "Source", select "Deploy from a branch"
4. Choose "main" branch and "/ (root)"
5. Save and wait a few minutes
6. Your quiz will be available at `https://yourusername.github.io/acronym-quiz`

### Option 2: Local Development

1. Clone the repository:
```bash
git clone https://github.com/yourusername/acronym-quiz.git
cd acronym-quiz
```

2. Open `index.html` in your browser:
```bash
# On macOS
open index.html

# On Linux
xdg-open index.html

# On Windows
start index.html
```

Or use a local server:
```bash
# Python 3
python -m http.server 8000

# Node.js with http-server
npx http-server
```

Then visit `http://localhost:8000`

## File Structure
```
acronym-quiz/
├── index.html                  # Main quiz application
├── acronym-quiz-data.json      # Quiz data (categories and acronyms)
└── README.md                   # This file
```

## How to Play

1. Select a category from the home screen
2. Type your answer for each acronym displayed
3. Press Enter or click "Submit Answer" to continue
4. Complete all 10 questions
5. Review your results and see correct answers
6. Play again or try a different category

## Customization

### Adding More Acronyms

Edit `acronym-quiz-data.json` and add entries to the relevant category:
```json
{
  "acronym": "API",
  "answer": "Application Programming Interface"
}
```

### Adding New Categories

1. Add a new category to the `categories` array:
```json
{
  "id": "newcategory",
  "name": "New Category Name",
  "icon": "🎯"
}
```

2. Add the acronyms data:
```json
"newcategory": [
  { "acronym": "XYZ", "answer": "Example Your Acronym" }
]
```

### Changing Number of Questions

In `index.html`, locate the `startQuiz()` function and modify the logic to select more or fewer questions from the category array.

### Styling

All CSS is embedded in `index.html` within the `<style>` tags. Modify colors, fonts, and layout there.

## Technical Details

- **Pure HTML/CSS/JavaScript** - No build process required
- **No external dependencies** - Everything runs client-side
- **Responsive design** - Works on all screen sizes
- **Accessible** - Keyboard navigation supported
- **Fast** - Loads instantly with minimal data transfer

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Guidelines

- Ensure all entries are actual acronyms (not brand names or single words)
- Verify acronym definitions are accurate
- Maintain consistent formatting in the JSON file
- Test the quiz before submitting

## License

This project is open source and available under the [MIT License](LICENSE).

## Credits

Created as an educational tool for testing professional acronym knowledge across various industries.

## Support

If you encounter any issues or have suggestions:
- Open an issue on GitHub
- Submit a pull request with improvements
- Star the repository if you find it useful!

## Roadmap

- [ ] Add difficulty levels (beginner, intermediate, expert)
- [ ] Implement leaderboard/high scores
- [ ] Add timer mode
- [ ] Support for multiple languages
- [ ] Dark mode
- [ ] Share results on social media
- [ ] Practice mode (review incorrect answers)
- [ ] Custom quiz creation

## Acknowledgments

Special thanks to all contributors who help maintain and expand the acronym database.

---

**Note:** Replace `yourusername` with your actual GitHub username in the URLs above.
