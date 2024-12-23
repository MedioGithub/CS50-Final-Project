# Mastermind Game

A Pokémon-themed **Mastermind** game built with C#. Players attempt to guess a secret code consisting of Pokémon names, receiving feedback on their guesses. The game supports single-player and multiplayer modes, features a scoring system, and offers a hint mechanism to enhance gameplay.

Created by Lorenzo Latinne, MedioGithub.

---

## Table of Contents

1. [Features](#features)
2. [Gameplay](#gameplay)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Project Structure](#project-structure)
6. [Controls](#controls)
7. [Customization](#customization)
8. [Contributions](#contributions)
9. [License](#license)
10. [Acknowledgements](#acknowledgements)

---

## Features

- **Single-player and Multiplayer Modes**: Play solo or with friends.
- **Dynamic Feedback**: Instant updates on the correctness of guesses.
- **Hints System**: Players can spend points to receive clues.
- **High Score Tracker**: Keeps track of the best player in multiplayer mode.
- **Timer-Based Gameplay**: Adds a layer of challenge with a countdown timer.
- **Customizable Attempts**: Choose the number of guessing attempts.
- **Debug Mode**: View the solution during development.

---

## Gameplay

1. Players are prompted to enter their usernames at the start.
2. Guess the secret code by selecting Pokémon from dropdown menus.
3. Receive feedback after each guess:
   - Correct Pokémon in the correct position.
   - Correct Pokémon in the wrong position.
   - Incorrect Pokémon.
4. Points are deducted for wrong guesses or purchasing hints.
5. The game ends when:
   - A player guesses the code correctly.
   - The maximum number of attempts is reached.
6. Multiplayer mode rotates between players, and the best performer is displayed at the end.

---

## Installation

### Prerequisites

- **Windows OS**
- [Visual Studio](https://visualstudio.microsoft.com/) with .NET Framework installed.

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/MedioGithub/CS50-Final-Project
2. Open the solution file (Mastermind.sln) in Visual Studio.
3. Build the project: Go to Build > Build Solution or press Ctrl + Shift + B.
4. Run the application: Press F5 or navigate to Debug > Start Debugging.

### Usage
1. Launch the application.
2. Enter usernames for the players.
3. Select Pokémon guesses using the dropdown menus.
4. Press Check Code to validate guesses.
5. View feedback and scores in the interface.
6. Repeat until the code is guessed or attempts run out.

### Project Structure

- MainWindow.xaml.cs: Core game logic, event handlers, and gameplay mechanics.  
- assets/choices/: Pokémon images used in the game.  
- assets/idle/: Placeholder images for unselected guesses.  
- High Scores Logic: Tracks and displays multiplayer results.  
- Game UI: Dynamically updates with player-specific information, scores, and feedback.

### Controls

- ComboBox Dropdown: Select Pokémon for each position.  
- Check Button: Validate your current guess.  
- Hints: Purchase hints for better guesses.  
- Keyboard Shortcut: Press Ctrl + F12 to toggle debug mode

### Customization

#### Add New Pokémon

1. Add Pokémon images to assets/choices/ folder in .png format.
2. Update the options array in MainWindow.xaml.cs:  
- string[] options = { "Bulbasaur", "Charmander", "Eevee", "Meowth", "Pikachu", "Squirtle", "YourNewPokemon" };  

#### Adjust Timer

Modify the totalTime variable in MainWindow.xaml.cs to set a new countdown duration:  

- TimeSpan totalTime = TimeSpan.FromSeconds(10); // Set to desired seconds  

### License

This project is licensed under the MIT License.

### Acknowledgements

Pokémon images are used under fair use for educational purposes.  
Inspired by the classic Mastermind board game.  
