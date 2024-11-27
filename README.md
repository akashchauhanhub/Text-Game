# Text-Game

The Adventure Game is an interactive text-based game built with Python and the tkinter library. The player makes choices that guide the storyline, with each decision leading to different outcomes. The game includes multiple story paths, and the player's choices determine whether they win or lose.

## Features
- Interactive Text-Based Gameplay: The game displays a story in a text area, and the player makes decisions by clicking buttons that represent choices.
- Multiple Story Paths: The game offers various paths depending on the player's choices, such as entering the forest, investigating noises, helping travelers, or finding magical stones.
- Winning and Losing Scenarios: Some choices lead to success, while others result in failure. The player can win by completing certain tasks or lose by making the wrong decisions.
- Play Again: After completing a game, the player can choose to play again by clicking the "Play Again" button.
## Installation
### Requirements
- Python 3.x: You need Python 3.x installed on your machine.
- Tkinter: Tkinter comes pre-installed with Python and is used to create the graphical user interface (GUI).
### Running the Game
- Save the Python code into a file named adventure_game.py.

- Open a terminal or command prompt.

- Navigate to the folder where adventure_game.py is located.

- Run the game with:


python adventure_game.py
```
This will open the graphical user interface (GUI) for the game.
```
## Gameplay Instructions
### Starting the Game
- When you first start the game, you will be welcomed and introduced to the story. You will have to make your first decision by choosing whether to:
      - Enter the forest
      - Walk around the forest
### Making Choices
- As you progress through the game, you'll be presented with various choices that affect the storyline. Each choice is displayed as a button, and you can click the button to proceed.
- Example choices include:
      - Investigate the noise or Ignore it and keep walking
      - Help the traveler or Leave them and walk away
      - Take the stone or Leave the stone and keep walking
## Winning and Losing
- The game features both winning and losing scenarios based on your decisions. If you make favorable choices, you'll find hidden treasures or powerful items that allow you to win. If you make poor choices, you might encounter dangerous situations or fall victim to wild animals, resulting in a loss.
### Playing Again
- After completing the game (either winning or losing), a Play Again button will appear, allowing you to start a new game from the beginning.
### Example Story Flow
- Start the Game: You are standing at the entrance of a dark forest. You can either:

      - Enter the forest: This leads you to investigate a noise, where you can either help a traveler or continue on your journey.
      - Walk around the forest: This leads you to a village, where you can choose to either enter or walk past it.
- Investigate the Noise: If you investigate the noise, you'll find a wounded traveler. You can choose to help them, which will reward you with a magical amulet and eventually lead to victory. Alternatively, if you leave them, you will encounter a dangerous cliff and lose the game.

- Ignore the Noise: If you ignore the noise, you discover a magical stone. You can choose to take the stone, which grants you power and leads to a victory, or leave it and continue, which results in a loss due to encountering a wild animal.

## Code Structure
### AdventureGame Class
The AdventureGame class is the core of the game. It contains all the logic for displaying the game story, handling user input, and updating the UI based on user choices.

#### Key Methods:
- __init__(self, root): Initializes the game, sets up the GUI, and calls start_game() to begin the adventure.
- start_game(self): Displays the initial story and offers the first set of choices.
- display_choices(self, choice1, choice2): Displays two buttons for the player to make a choice.
- handle_choice(self, choice): Handles the choice the player makes and directs the game to the appropriate next step.
- enter_forest(self), walk_around_forest(self), etc.: These methods represent different parts of the story and the consequences of the player's choices.
### Tkinter Widgets
- Text Widget: Used to display the game story and options.
- Button Widgets: Used to display choices for the player. Each button corresponds to an option that leads the player to a new part of the story.
- Frame: A container for the buttons, allowing for better organization and layout control.
### Game Flow Example
- Choice 1: Enter the forest → Investigate the noise → Help the traveler → Win the game
- Choice 2: Walk around the forest → Enter the village → Win the game
- Choice 3: Ignore the noise → Take the stone → Win the game
- Choice 4: Leave the traveler → Fall off a cliff → Lose the game
- Choice 5: Leave the stone → Get attacked by a wild animal → Lose the game
