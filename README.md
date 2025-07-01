🕹️ How Does "Assembly Endgame" Work?
Assembly Endgame is a browser-based word guessing game inspired by the classic game Hangman — with a developer twist. The player’s goal is to guess a hidden programming language name (e.g., javascript, python, csharp) by selecting letters from a virtual keyboard.

🔄 Gameplay Flow:
On game start, a word is randomly selected from a predefined list of programming languages.

The word is displayed as a series of blanks (_ _ _ _ _), one underscore per letter.

The player clicks letters on the on-screen keyboard:

Correct guess: The letter is revealed in the correct position(s).

Wrong guess: The player loses one of a limited number of lives (attempts).

The game ends when:

The player guesses the entire word – a victory message with confetti appears.

The player runs out of lives – a defeat message with programming humor is shown (e.g., "Your code didn’t compile").

🔑 Key Features:
🔠 Interactive virtual keyboard – letters are disabled after being clicked; visual feedback shows which letters were correct or incorrect.

🧠 Real-time game state updates – all game data (word progress, used letters, lives left) is managed with React state and updates instantly.

🎉 Victory animation – uses the react-confetti library for a fun and rewarding win effect.

🔁 "New Game" button – instantly resets the game and loads a new random word.

🧩 Game Logic Overview:
The entire logic is written in vanilla React.js, using useState and useEffect to manage:

The current word to guess

Clicked letters (correct and incorrect)

Remaining lives

Game-over and win conditions

The code is organized into clean, modular components with separation of concerns between UI (App.js), logic (utils.js), and styling (App.css).
