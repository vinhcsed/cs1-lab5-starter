# CS1: Lab 5

## Setup
1. Update the contents of *ID.txt* with your identifier (school email **without @school.edu**).
2. Write pseudocode for your program in *PSEUDO.txt*.

## How to Run Your Program
* [**WINDOWS**]
   - In VSCode, press the play button in the top right corner (it should appear when you open a `.cpp` file). Your program should compile and run.
   - Alternatively, open a terminal. Type `make.bat` and press return. Your program should compile and run.
* [**MAC/LINUX**]
   - Open a Terminal. Type `make` and press return. Your program should compile and run.

## Assignment Specification
### The Elements Game
* Implement this program in `main.cpp`.
* This program will be a variation on the classic game Rock, Paper, Scissors.
* There are four choices: Air, Water, Earth, or Fire
   - Air *gusts* Earth
   - Water *extinguishes* Fire
   - Earth *absorbs* Water
   - Fire *burns* Air
   - An element draws with itself
* *Continuously* display a menu of options and prompt the user to make a selection.
   - `A` for Air, `W` for Water, `E` for Earth, `F` for Fire
   - The user should be continuously prompted until they make a valid selection
* After the user has made their selection, the program should **randomly** select another element.
   - Randomness can be accomplished using `rand()` and `srand()` from the `<cstdlib>` library
* Output a message to the terminal determining if the user has won or lost the match.
* Lastly, after the winner is determined, the user should select whether or not to play again.
   - `Y` to play again, or any other key to quit

### Function Requirements
This starter code includes function prototypes to help you get started. Each of these functions must be defined and used in the final program. Additional helper functions should be defined if necessary.
* `char userChoice()`
  - Continuously prompts the user for a selection until a valid choice is made, then returns that character choice
* `char computerChoice()`
  - Generates a random choice (A, W, E, or F) and returns it
* `void determineWinner(char, char)`
  - Determines the winner of a match between two element choices and displays it
* `bool playAgain()`
  - Prompts the user to ask if they want to play again (returns `true`) or not (returns `false`)

#### Example
```
ELEMENTS: AIR (A), WATER (W), EARTH (E), FIRE (F)
Select your element: A
You chose AIR. Your opponent chose AIR.
Draw!
Would you like to play again? (Y for yes, other key to quit): Y

ELEMENTS: AIR (A), WATER (W), EARTH (E), FIRE (F)
Select your element: X
Invalid selection, try again: Y
Invalid selection, try again: A
You chose AIR. Your opponent chose EARTH. AIR gusts EARTH.
You win!
Would you like to play again? (Y for yes, other key to quit): Y

ELEMENTS: AIR (A), WATER (W), EARTH (E), FIRE (F)
Select your element: F
You chose FIRE. Your opponent chose WATER. WATER extinguishes FIRE.
You lose!
Would you like to play again? (Y for yes, other key to quit): Y

ELEMENTS: AIR (A), WATER (W), EARTH (E), FIRE (F)
Select your element: E
You chose EARTH. Your opponent chose WATER. EARTH absorbs WATER.
You win!
Would you like to play again? (Y for yes, other key to quit): Y

ELEMENTS: AIR (A), WATER (W), EARTH (E), FIRE (F)
Select your element: E
You chose WATER. Your opponent chose EARTH. EARTH absorbs WATER.
You lose!
Would you like to play again? (Y for yes, other key to quit): Q
```

## Submission
1. Remember to *commit* and *push* your changes to this repository.
