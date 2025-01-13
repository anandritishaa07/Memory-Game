Simon Says Game 🎮
A fun and interactive "Simon Says" memory game built using HTML, CSS, and JavaScript. Test your memory and reflexes as the game sequence grows longer with each level!

📂 Project Structure
bash
Copy code
MemoryGame/
├── index.html        # Main HTML file
├── simonsayscss.css  # Stylesheet for the game
├── simonsaysjs.js    # JavaScript file for game logic
└── README.md         # Project documentation
🚀 Features
Interactive Gameplay: Users must repeat the sequence of button flashes in the correct order to progress.
Dynamic Levels: The sequence grows longer with each level, increasing difficulty.
Visual Feedback: Buttons flash to indicate the sequence or user input, enhancing usability.
Game Over Screen: Displays the final score and allows restarting the game.
Responsive Design: Works seamlessly across different devices.
🛠️ Technologies Used
HTML5: Markup for the game structure.
CSS3: Styling and animations for a visually appealing interface.
JavaScript: Handles game logic, user interaction, and dynamic updates.
🎮 How to Play
Press any key to start the game.
Watch the button sequence flash on the screen.
Click the buttons in the exact order they were shown.
Progress to the next level if you succeed; otherwise, see your final score and restart.


🧩 Code Highlights
Flash Animation
javascript
Copy code
function gameFlash(btn) {
  btn.classList.add("flash");
  setTimeout(() => btn.classList.remove("flash"), 250);
}
Level Up Logic
javascript
Copy code
function levelUp() {
  userSeq = [];
  level++;
  h2.innerText = `Level ${level}`;
  let randColor = btns[Math.floor(Math.random() * btns.length)];
  gameSeq.push(randColor);
  console.log(gameSeq);
  gameFlash(document.querySelector(`.${randColor}`));
}
🛠️ Setup and Usage
Clone the repository:
bash
Copy code
git clone https://github.com/anandritishaa07/Memory-Game.git
Navigate to the project folder:
bash
Copy code
cd Memory-Game
Open index.html in a web browser to start the game.
🌟 Lessons Learned
Gained hands-on experience with DOM manipulation and event handling in JavaScript.
Learned to implement dynamic game logic and provide feedback through animations.
Improved understanding of modular and reusable code practices.
📜 License
This project is open-source and available under the MIT License. Feel free to contribute or adapt it for your needs!

