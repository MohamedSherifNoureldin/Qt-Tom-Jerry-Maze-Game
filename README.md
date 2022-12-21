# Qt Tom & Jerry Maze Game
A C++ Qt game based on the classic Tom & Jerry cartoon but with a theme of playing in space. The goal is to have Jerry escape the maze before Tom Catches him. The game is based on the A* Graph algortihm to let Tom automatically try to catch Jerry in the shortest time and path possible. This game was created as a project for the  Fundamentals of Computing II course (CSCE1101).

## Features
- Leaderboard that keeps track of Scores
- Ability to increase the number of Tom's to increase the difficulty
- Ability to increase the speed of Tom to increase the difficulty
- Powerups to make Jerry invincible for a short period of time
- Tom automatically tries to catch jerry using A* Graph Algorithm
- Object Oriented Programming

## Code Files Explained
- main: The main file that runs the game
- welcomescreen: The welcome screen that allows the user to choose the username, number of Tom's and dificulty
- gamescreen: The game screen that displays the game and the maze
- gamefinishscreen: The game finish screen that displays whether the player won or lost and the option to view the leaderboard or play again
- leaderboard: the leaderboard screen that displays the scores of the players
- user: The user class that stores the username and score of the player
- character: The character class that acts as the parent for both Tom and Jerry. It stores the position, direction, and the image of the character along with it being able to move the character
- item: The item class that acts as the parent for the powerup and cheese items. It stores the position and the image of the item.
- map: The map class that takes the map data to build the adjaceny matrix and calculate the shortest path for Tom to catch Jerry.
- countinglabel: The counting label class that is used to display the number of lifes, and cheese left for Jerry.
- tom: The tom class that inherits from the character class.
- jerry: The jerry class that inherits from the character class.
- powerup: The powerup class that inherits from the item class.
- cheese: The cheese class that inherits from the item class.

## Game Resources Explained
- blackBackground.jpg: A black background image having some starts to act as the background of the game.
- cheese.png: The image of the cheese item.
- edgeCornerBorder.jpg: The image of the corner border of the maze.
- GameOver.png: The image of the game over screen.
- head.png: The image of the space helment.
- horizontalBorder.jpg: The image of the horizontal border of the maze.
- jerryNormal.png: The image of the normal jerry running without powerup or cheese.
- jerryNormalCheese.png: The image of the normal jerry running while holding cheese.
- jerryStrong.png: The image of the powered up jerry running without cheese.
- jerryStrongCheese.png: The image of the powered up jerry running while holding cheese.
- jerryWon.png: The image of the winning screen.
- leaderBoard.txt: The text file that stores the scores of the players. Each line holds the usrname and score of the player seperated by a space.
- loseScreen.png: same as GameOver.png
- map.txt: The text file that stores the map data. Each line holds the data of a row of the maze. The data is seperated by a space. The data is as follows:
  - -1: Solid Wall -> solidBorder.jpg
  - -2: Horzontal Border in middle of the maze -> horizontalBorder.jpg
  - -3: Vertical Border in middle of the maze -> horizontalBorder.jpg but rotated 90 degrees
  - -4: Intersection of 3 borders -> tCornerBorder.jpg but rotated 90 degrees
  - -5: Intersection of 3 borders -> tCornerBorder.jpg but rotated 270 degrees
  - -6: Intersection of 3 borders -> tCornerBorder.jpg unrotated
  - -7: Intersection of 3 borders -> tCornerBorder.jpg but rotated 180 degrees
  - -8: Intersection of 2 borders (edge) -> edgeCornerBorder.jpg
  - -9: Intersection of 2 borders (edge) -> edgeCornerBorder.jpg but rotated 90 degrees
  - -10: Intersection of 2 borders (edge) -> edgeCornerBorder.jpg but rotated 180 degrees
  - -11: Intersection of 2 borders (edge) -> edgeCornerBorder.jpg but rotated 270 degrees
  - -20: Location of Home of Jerry -> blackBackground.jpg (has no special design)
  - zero or +ve number: Normal blocks -> blackBackground.jpg
- powerUp.png: The image of the powerup item.
- solidBorder.jpg: The image of the solid border of the maze.
- tCornerBorder.jpg: The image of the intersection of 3 borders of the maze.
- tom.png: The image of Tom.
- welcomeScreen.png: The image of the welcome screen.
- windScreen.png: The image of the winning screen.
