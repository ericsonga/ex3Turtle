..  Copyright (C)  Mark Guzdial, Barbara Ericson, Briana Morrison
    Permission is granted to copy, distribute and/or modify this document
    under the terms of the GNU Free Documentation License, Version 1.3 or
    any later version published by the Free Software Foundation; with
    Invariant Sections being Forward, Prefaces, and Contributor List,
    no Front-Cover Texts, and no Back-Cover Texts.  A copy of the license
    is included in the section entitled "GNU Free Documentation License".

.. setup for automatic question numbering.

.. 	qnum::
	:start: 1
	:prefix: 4-4-
	
.. |runbutton| image:: Figures/run-button.png
    :height: 20px
    :align: top
    :alt: run button
	
.. |pass| image:: Figures/pass.png
    :height: 20px
    :align: top
    :alt: pass
    
.. |start| image:: Figures/start.png
    :height: 24px
    :align: top
    :alt: start
    
.. |finish| image:: Figures/finishExam.png
    :height: 24px
    :align: top
    :alt: finishExam
    
.. |right| image:: Figures/rightArrow.png
    :height: 24px
    :align: top
    :alt: right arrow for next page
    
.. |checkme| image:: Figures/checkMe.png
    :height: 20px
    :align: top
    :alt: check me

Example 4: Stamp an X
---------------------------------------
      
You can use the ``goto(x,y)`` function to move to a particular x and y position.  The center of the drawing area is at (0,0).  You can use ``color("aColor")`` to change the drawing or stamping color.

Run Code
=========

Click the |runbutton| button to see the turtle stamp an X shape.

.. activecode:: Stamp_X
   :nocodelens:

   from turtle import *
   space = Screen()
   nick = Turtle()
   
   # setup for first line
   nick.shape("turtle")
   nick.penup()
   nick.goto(-150,-150)
   nick.left(45)

   # stamp the blue line
   nick.color("blue")            
   for num in range(15):  
       nick.stamp()
       nick.forward(30)
   nick.goto(150,-150)
   nick.left(90)

   # stamp the green line
   nick.color("green")
   for num in range(14):  
       nick.stamp() 
       nick.forward(30)
   
Practice 4: Stamp Two Squares
------------------------------

Use the turtle to stamp two squares of turtles using two different colors.
   

Order Code Here
================

Click on the |start| button below when you are ready to try to order this code.  You will have up to 10 minutes to try to solve it.  Click the |runbutton| button to check your solution.  Click on the |finish| button when you have solved this problem or wish to move on without solving it.

.. timed:: turtle_squares_timed
   :timelimit: 10
   :noresult:
   :nofeedback:
   :fullwidth:
   
   .. parsonsprob:: inst4_turtle_two_squares
      :order: 13, 9, 4, 3, 11, 8, 0, 12, 10, 2, 1, 7, 5, 6
      :adaptive:

      The following program uses the stamp method to create two squares of turtle shapes as shown to the left, <img src="./_static/TurtleStampDoubleSquare.png" width="150" align="left" hspace="10" vspace="5" /> but the lines are mixed up.  The program should do all necessary set-up, create the turtle, set the shape to "turtle", and pick up the pen.  Draw the blue square before you draw the green one.<br /><br /><p>Drag the needed blocks of statements from the left column to the right column and put them in the right order with the correct indention.  Click on <i>Check Me</i> to see if you are right. You will be told if any of the lines are in the wrong order or are the wrong blocks.</p>
      -----
      from turtle import *
      space = Screen()
      =====
      nick = Turtle()
      nick.shape("turtle")
      =====
      nick.penup()
      =====
      nick.penUp() #paired
      =====
      nick.goto(-150,-150)
      nick.left(90)
      =====
      nick.goto(-150,-150)
      nick.right(90) #paired
      =====
      nick.color("blue")            
      for count in range(4):
          for num in range(5):
              nick.stamp()
              nick.forward(30)
          nick.right(90)
      =====
      nick.goto(-120,-120)
      nick.color("green")            
      for count in range(4):
      =====
      nick.goto(120,-120)
      nick.color("green")            
      for count in range(4): #paired
      =====
          for num in range(3):
      =====
          for num in range(2): #paired
      =====
              nick.stamp()
              nick.forward(30)
      =====
          nick.right(90)
      =====
          nick.left(90) #paired
 

When you are finished with this problem, or are ready to move on, click the |finish| button and then go to the next page by clicking the right arrow |right| near the bottom right of this page.    
