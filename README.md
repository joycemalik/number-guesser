# Number Guessing Game

A simple web-based game where the player attempts to guess a randomly generated number between 1 and 100. It provides feedback on guesses, tracks attempts, and allows for game resets.

## How to Use

1.  Save the provided HTML content as `index.html` in a file.
2.  Open `index.html` in your web browser.
3.  Enter a number between 1 and 100 in the input field and click "Guess" or press Enter.
4.  Follow the feedback ("Too high", "Too low") to narrow down your guess.
5.  The game will tell you when you've guessed correctly and how many attempts it took.
6.  Click "Reset Game" to start a new round.

## Code Explanation

*   **HTML:** Sets up the basic game layout, including a title, instructions, an input field for guesses, a "Guess" button, a "Reset Game" button, and paragraphs to display feedback and the number of attempts.
*   **CSS:** A small `<style>` block embedded in the `<head>` provides basic styling for a clean, centered layout with distinct buttons, enhancing readability and user experience.
*   **JavaScript:**
    *   `targetNumber`, `attempts`, and `gameOver` variables manage the game state.
    *   `initializeGame()`: Resets the game by generating a new random number, clearing attempts, enabling the input field and guess button, and disabling the reset button until a game is in progress or won.
    *   `checkGuess()`: Validates user input, increments attempts, compares the guess to the `targetNumber`, and updates the feedback message. If the guess is correct, it disables further input/guesses and enables the reset button.
    *   Event listeners are set up for the "Guess" button (click), the input field (Enter key for convenience), and the "Reset Game" button (click) to trigger the game logic.

## License

This project is licensed under the MIT License.