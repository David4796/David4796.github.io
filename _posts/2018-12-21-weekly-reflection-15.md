---
layout: post
title: "My Video Game Project"
date: 2019-3-09
---

Shared link to my game:
https://www.wescheme.org/view?publicId=lRg67RFADP

Game's Title: 
Robo's Adventure
 
 Here is a Screenshot of my game:
 * * *
![MyGame](/images/image.png)
* * *
 
 
  The setting of my game is in the swamp my character is a robot that is trying to collect batteries in order to earn points and is also trying to avoid buckets of water along the way so he doesn’t lose any points.

This is my update-player function with its contract, purpose statement, examples and definition. 

(EXAMPLE (update-player   30 40 "up")  (make-posn 30 140))
(EXAMPLE (update-player   60 50 "up")  (make-posn 60 150))

(EXAMPLE (update-player 300 200 "down") (make-posn 300 100))
(EXAMPLE (update-player 500 300 "down") (make-posn 500 200))

(EXAMPLE (update-player 700 800 "right") (make-posn 800 800))
(EXAMPLE (update-player 800 500 "right") (make-posn 900 500))

(EXAMPLE (update-player 100 700 "left") (make-posn  0 700))
(EXAMPLE (update-player 600 900 "left") (make-posn 500 900))

1. ; update-player : Number String Number String -> Number Number

2. (define (update-player x y key) 
3.   (cond
4.     [(string=? key    "up")  (make-posn  x (+ y 100))]
5.     [(string=? key  "down")  (make-posn  x (- y 100))]
6.     [(string=? key "right")  (make-posn (+ x 100)  y)]
7.     [(string=? key  "left")  (make-posn (- x 100)  y)]
8.     [else (make-posn x y )]))

  
  The EXAMPLES in my function allow me to know if my function is working the way that I wanted it too. Line 0 tells us what the function does which is take in two numbers and two strings and produces two numbers. Line 1 tells what the functions name is and what the variables are going to be called. Line 2 is the beginning of condition which means that there are some things that have to be met in order for the function to work. Lines 3, 4, 5, and 6 are clauses or the conditions that should be met in order for something to happen in this case make the character move left, right, up, or down. Line 7 is when the conditions that were set for the function weren’t met and so then this will happen in this case if I don’t press up, down, left or right then the character will just stay in place nand not move. The role of the update-player function is that it allows for the player to make the character either go up, down, left,or right by increasing or decreasing the position of the character by 100. Making the character go up or down would mean to change the y value of the character and making the character go left or right meant that the x value of the character had to change. This function also allows for the character to avoid the dangers of the game and to get points in the game.
