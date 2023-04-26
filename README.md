# Pong-game-
Pong is a classic and iconic video game that has become a part of gaming
history. Developed and released by Atari in 1972, it was one of the first arcade
games to gain widespread popularity and was instrumental in launching the video
game industry.
The game is played by two players, each with a paddle. The players use their
paddles to hit a small ball back and forth across the screen. The paddles can be
moved up and down to control the direction of the ball. The aim of the game is to
make the ball go past the other player's paddle to score a point. The game
continues until one player reaches a certain number of points, usually 11 or 21.
Pong may seem like a simple game, but it has a lot of depth and strategy.

The program defines several user-defined functions that are used in the main
function to create and run the Pong game:
1.drawBoard(): This function is used to draw the game board and paddles. It first
clears the color buffer using glClear(GL_COLOR_BUFFER_BIT). It then sets the
color to white and draws two rectangles to represent the paddles. Finally, it sets
the color to red and draws a solid sphere to represent the ball.
2.update(int value): This function is used to update the game physics and ball
movement. It first moves the ball by updating its ballX and ballY positions based
on its current ballDX and ballDY velocities. It then checks for collision with the top
or bottom of the screen and changes the direction of the ball's ballDY velocity if
necessary. It also checks for collision with the paddles and changes the direction
of the ball's ballDX velocity if necessary. Finally, it checks for scoring and updates
the score and ball position accordingly. It then posts a redisplay to redraw the
board and sets a timer for the next update.
3.keyboard(int key, int x, int y): This function is used to set up the keyboard
controls for the game. It takes in the key pressed as an integer and updates the
position of the paddles accordingly. If a paddle reaches the top or bottom of the
screen, it is kept within bounds.
All of these functions are then called in the main function to set up the game
window and run the game loop using glutMainLoop(). The program also defines
several constants and variables to be used throughout the game.

