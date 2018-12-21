---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## The United Kingdom Flag

## Describe your program

I designed a Program to make the flag of the United kingdom.To be honest I will probably get a grade of 2 or above because I was able to to make the United Kngdom Flag and was able to find a way to scale.


## Current output

* * *
![MyFlag](/images/flagV2.png)
* * *

## Describe your process.

Some advise a student gave me that helped me make the United Kingdom Flag was to make all of the diagonal lines on the flag seperatly so that it's a lot easier to do and also because if look at the United Kingdom Flag those lines are in different positions and not just one straight line.

 


## Explain your code.

* * *

```
(define size 100)

(define width (* 5 size))                    
(define height (* 3 size))

(define w2 (* 2.5 size)) (define h2 (* .2 size))

(define w3 (* 6 size)) (define h3 (* .55 size))

(define w4 (* 6 size)) (define h4 (* .5 size))

(define w5 (* 7 size)) (define h5 (* .85 size))

(define w7 (* 2.5 size)) (define h7 (* .2 size))

```

* * *

-   Explain the code you posted by telling us about each argument.
-   Then tell us how your code section fits into the whole.
 
In these lines of code as you can see I defined size as 100 meaning that everytime I use size in an expression the computer will read it as 100. To scale my flag all I would have to do is change 100 to whatever number I want and that will either increase or decrease the size of the flag since it is multiplying a number I want the shape to be by size(which can be any number I want it to be) it will change the flag to be how I wnat it to be.


## Program code

```
(define size 100)

(define width (* 5 size))                    
(define height (* 3 size))

(define w2 (* 2.5 size)) (define h2 (* .2 size))

(define w3 (* 6 size)) (define h3 (* .55 size))

(define w4 (* 6 size)) (define h4 (* .5 size))

(define w5 (* 7 size)) (define h5 (* .85 size))

(define w7 (* 2.5 size)) (define h7 (* .2 size))

(define w8 (* 3.7 size)) (define h8 (* .2 size))              
             
(define X (* 2.5 size))
(define Y (* 1.5 size)) (define Y2 (* 1.5 size))

(define X3 (* 1 size)) (define Y3 (* 2.3 size))

(define X4 (* 4.2 size)) (define Y4 (* .6 size))

(define X5 (* .41 size)) (define Y5 (* .2 size))

(define X6 (* 3.79 size)) (define Y6(* 2.3 size))

;United Kingdom flag 
;red cross
(put-image(rotate 90(rectangle w3 h3 "solid" "red")) X Y (put-image(rectangle w4 h4 "solid" "red") X Y2
;white cross                                                                        
(put-image(rotate 90(rectangle w5 h5 "solid" "white")) X Y (put-image(rectangle w5 h5 "solid" "white") X Y2 
;top left and bottom right                                                                        
(put-image(rotate 150(rectangle w7 h7 "solid" "red"))X3 Y3(put-image(rotate 150(rectangle w7 h7 "solid" "red")) X4 Y4 

                                                                               ;top right and bottom left                                                         
(put-image(rotate 390(rectangle w8 h8 "solid" "red")) X6 Y6 (put-image(rotate 391(rectangle w8 h8 "solid" "red")) X5 Y5 
;white X                                                                        
(put-image(rotate 150(rectangle w4 h4 "solid" "white")) X Y (put-image(rotate 390(rectangle w4 h4 "solid" "white")) X Y 
                                                                           
(rectangle width height "solid" "blue")))))))))))
```
