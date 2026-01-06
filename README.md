# 🧠 React Quiz App

A modern, interactive quiz application built with React that tests your knowledge of React concepts. Features a timed quiz experience with progress tracking, score calculation, and high score persistence.

![React](https://img.shields.io/badge/React-18.2.0-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![JSON Server](https://img.shields.io/badge/JSON_Server-0.17.3-green?style=for-the-badge)

## ✨ Features

- **📚 Multiple Choice Questions** - Test your React knowledge with carefully crafted questions
- **⏱️ Timed Quiz** - Challenge yourself with a countdown timer
- **📊 Progress Tracking** - Visual progress bar showing your advancement through the quiz
- **🏆 Score System** - Points-based scoring with different values per question
- **🥇 High Score** - Track your best performance across sessions
- **🔄 Restart Capability** - Retake the quiz to improve your score
- **⚡ Real-time Feedback** - Instant visual feedback on correct/incorrect answers

## 🛠️ Tech Stack

- **Frontend:** React 18 with Hooks
- **State Management:** React Context API + useReducer
- **Backend:** JSON Server (for quiz questions API)
- **Styling:** CSS3 with modern design patterns
- **Testing:** Jest & React Testing Library

## 📁 Project Structure

```
react-quiz/
├── public/
│   ├── questions.json      # Quiz questions data
│   └── ...
├── src/
│   ├── components/
│   │   ├── App.js          # Main application component
│   │   ├── Header.js       # App header with logo
│   │   ├── Main.js         # Main content wrapper
│   │   ├── StartScreen.js  # Welcome screen
│   │   ├── Question.js     # Question display
│   │   ├── Options.js      # Answer options
│   │   ├── Progress.js     # Progress bar
│   │   ├── Timer.js        # Countdown timer
│   │   ├── NextButton.js   # Navigation button
│   │   ├── FinishScreen.js # Results screen
│   │   ├── Footer.js       # Footer wrapper
│   │   ├── Loader.js       # Loading spinner
│   │   └── Error.js        # Error display
│   ├── contexts/
│   │   └── QuizContext.js  # Global state management
│   ├── index.js            # App entry point
│   └── index.css           # Global styles
└── package.json
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/mohamedosama2004/react-quiz.git
   cd react-quiz
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the JSON Server** (in one terminal)
   ```bash
   npm run server
   ```
   This starts the questions API at `http://localhost:9000`

4. **Start the React app** (in another terminal)
   ```bash
   npm start
   ```
   The app will open at `http://localhost:3000`

## 📜 Available Scripts

| Command | Description |
|---------|-------------|
| `npm start` | Runs the app in development mode |
| `npm run server` | Starts JSON Server on port 9000 |
| `npm test` | Launches the test runner |
| `npm run build` | Builds the app for production |
| `npm run eject` | Ejects from Create React App |

## 🎮 How to Play

1. Click **"Let's start"** on the welcome screen
2. Read each question carefully
3. Select your answer from the multiple choices
4. Click **"Next"** to proceed to the next question
5. Keep an eye on the timer! ⏰
6. View your final score and compare with your high score
7. Click **"Restart quiz"** to try again

## 🏗️ Architecture

The app uses the **Context API** with **useReducer** for state management, providing:

- Centralized state for quiz data
- Clean separation of concerns
- Predictable state updates
- Easy debugging and testing

### State Structure
- `questions` - Array of quiz questions
- `status` - Current app status (loading, error, ready, active, finished)
- `index` - Current question index
- `answer` - User's selected answer
- `points` - Accumulated score
- `highscore` - Best score achieved
- `secondsRemaining` - Timer countdown

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Built as part of learning React advanced patterns
- Inspired by modern quiz applications
- Thanks to the React community for excellent documentation

---

<p align="center">
  Made with ❤️ and React
</p>