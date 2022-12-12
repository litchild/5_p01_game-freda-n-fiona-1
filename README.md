# Project 01 For NeXT CS
### Class Period: 05
### Name0: Fiona Zhang
### Name1: Freda Dong
---


Your mission is to recreate one of these two classic arcade games:
- Breakout/Arkanoid [demo 0](https://elgoog.im/breakout/)  [demo 1](https://www.crazygames.com/game/atari-breakout)
- Space Invaders [demo 0](https://elgoog.im/space-invaders/) [demo 1](https://www.crazygames.com/game/space-invaders)

This project will be completed in phases. The first phase will be to work on this document. Use makrdown formatting. For more markdown help [click here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) or [here](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)


---

## Phase 0: Game Selection, Analysis & Plan

#### Selected Game: Breakout/Arkanoid

### Necessary Features
What are the core features that your game should have? These should be things that __must__ be implemented in order to make the game playable, not extra features that could be added to make the game more fun to play.

Three different objects that represent the player controlled paddle, a ball, and the layers of bricks. The ball should bounce off the paddle and walls and break the bricks when in contact, and the speed of the ball will increase. When the ball falls to the bottom of the screen past the paddle it resets but the bricks remain the same and the game continues. 

### Extra Features
What are some features that are not essential to gameplay, but you would like to see (provided you have time after completing the necessary features.

A score for when bricks are broken, different speed increases depending on what layer of bricks were broken, and limited rounds (ie. if the ball hits the bottom of the screen three times everything resets). 


### Controls
How will your game be controlled? If the mouse will be used, explain how. List all keyboard commands as well.

Keyboard Commands:
- r = reset the entire game

Mouse Conrol:
- Mouse movement: moving the paddle (mouseX will be equal to the location of the paddle's center)
- Mouse pressed: start the ball moving (


### Classes
What classes will you be creating for this project? Include the instance variables and methods that you believe you will need. You will be required to create at least 2 different classes. If you are going to use classes similar to those we've made for previous assingments, you will have to add new features to them.

Ball
- Instance variables:
  - x, y
  - r (radius)
  - xvelocity, yvelocity
- METHODS
  - move
  - display
  - reset
  - bounce

Paddle
- Instance variables:
  - paddleWidth, paddleHeight
  - px, py
- METHODS
  - move
  - display
  - paddleCollide (have to divide into three sections for bounce) 
  - reset 

Bricks (will be array)
- Instance variables:
  - brickHeight, brickWidth (note: will be randomized)
  - bx, by
  - nextbx, nextby 
- METHODS
  - display
  - ballCollide 
  - reset 
  - randomizedBricks

