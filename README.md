# Wheel-of-Fortune

## INSTRUCTIONS TO PLAY
*  Double-click Wheel_of_Fortune.py
* The game will now run and start another graphics window.
* Keep the Python shell on one side and the graphics window on the other side (resize window if you want to).
* Enjoy playing the game!
#### Important notes
* The game does not tell you which letters have already been guessed before, so be attentive even when it is not your turn.
*  This game is meant for three players only.
*  The Python shell will take your input, the graphics window is only to enhance your gaming experience, it doesn’t take input.
*  The graphics window may look frozen sometimes, but it will update once you have provided the input. Please don't try and close it.
*  Please make sure that phrases.txt and wheel.gif are in the same folder as the game before running it.

## ABOUT THE GAME
  The game uses the built-in python modules only. It uses the turtle module to make all the graphics appear on a separate window. The code utilises many functions that can be loosely divided into:
* Turtle/ graphics functions
* Gameplay functions
There are comments in the code explaining what each function does.

### Features of turtle graphics
*  The turtle graphics have boxes for each letter in the phrase, printing the boxes in two lines if the phrase is too long.
*  The wheel on the turtle screen doesn’t spin, instead the pointer spins around the wheel.
*  Where the pointer stops spinning is determined by the spin variable that is randomly chosen from the wheel list.
*  The letters slowly fill in whenever the player guesses right.
*  The player score on top of the screen updates whenever a player gets money or loses money.
*  There is graphics congratulating whichever player wins once the game ends. This graphic also displays the boxes, showing the completed phrase and the amount of money won.
*  Most of the turtle objects are used by many functions and hence, are assigned to the global namespace. This makes it easy for all functions to access the turtles.

### Features of gameplay
*  The main function of the game is play(), this calls the other two most important functions, spin_turn() and choose(). spin_turn() and choose() decide what to do based on the inputs given by the player.
*  The gameplay is done through a series of if/else statements and according function calls.
*  The whole game is run through a while loop that calls play() and loops as long as no player has guessed the phrase.
*  Boolean variables like nextPlayer and rightGuess are used to determine whether the code should continue to loop through the players.
*  The game outputs appropriate error messages if there is a wrong type of input.
*  The phrase is read using the file method readline(), using randint() to get a random line.
  
### Some problems overcome
*  Global variables are used quite a bit in this program. This is due to the fact that these variables are used by more than two or three functions and passing them as parameters makes the code more complicated. Hence, global namespace is used to be more efficient.
*  Passively timed input is used in this game. Other solutions found for actively timed input, either used modules that are not built-in or used input that was restricted to one OS (this meant the game couldn’t be run on all computers) or wasn’t user friendly (used Command-line to run the game). Thus, passively timed input is used as it is most efficient.
