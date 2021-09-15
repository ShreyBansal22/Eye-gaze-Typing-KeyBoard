

## Title: EYEGAZE KEYBOARD TYPING

## Motivation : 
The idea of this project comes while reading a Research Paper of OpenCV[1] , The project is totally made to help those who have disablility in communication while 
giving information to other.To make communication easier, some people who are unable to speak or has some disability in motor operation especially hand this project
is dedicated to them.

## Methodology :
This project is made mainly in two parts:
  1. Designing a keyboard with keys and cursor moving
  2. Typing on board while one blink eyes.

  ## 1. Designing a keyboard:
        As we now that there are 26 letters and it is not easier and effecient to incorporate them in a single screen of keyboard. So the keyboard is divided into 2 splits namely as 
        left and right . Left set contains the keys of left part of the keyboard like(Q-T,A-G,Z-V) likewise the other part is made. These operations are simply done by making a dictionary
        of keys and simple numpy and openCV operations.
        Apart from making the keyboard there is a cursor which when moves over the keyboard the keys lit up. The light is lit-up for 10 frames on each key and then moves forward.
        
  ## 2. Typing on Keyboard using EyeGaze:
        For detecting the facial points of the eye , a famous library D-lib is used which distinguishes and helps is marking out the eye points. extreme left and extreme right points are
        taken to make a horizontal line and mid top and mid bottom points are taken to make vertical line.
        
        As the keyboard is divided into two parts (i.e left and right) we open that segment by moving the eyegaze . As we saw towards left then all of our eye part is white so we do thresholding
        into it so that left part gets open and do viceversa for other.
        
        To type on keyboard blink is used such that when the vertical distance becomes zero for some specified seconds a blink gets counted and the word gets typed.


      

        
For downloading Dlib I have wrote a piece you can refer to it.

        
        
        

[1] https://ieeexplore.ieee.org/document/7860997
