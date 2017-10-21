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
	:prefix: 4-3-
	
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
    
Example 3: Stamping with Turtles
--------------------------------------------------

You can change the shape of the turtle using the ``shape`` procedure.  In the program below we set it to look more like a turtle.  

A turtle can also **stamp** a copy of itself on the screen (turtle drawing area), and this will remain after the turtle has moved somewhere else.  Do this with the ``stamp`` procedure.  Stamping works even when the pen is up.  You can ask the turtle to pick up the pen using ``penup()`` as shown below.  When the pen is up the turtle will not draw a line when it moves.


Run Code
=========

Click the |runbutton| button to watch the turtle stamp out a spiral shape.

.. activecode:: stamp_spiral
   :nocodelens:

   from turtle import *
   space = Screen()
   tess = Turtle()
   tess.shape("turtle")

   tess.penup()                  # ask tess to pick up her pen 
   for size in range(5, 60, 2):  # start with size = 5 and grow by 2
       tess.stamp()                # leave an impression on the canvas
       tess.forward(size)          # move tess along
       tess.right(24)              # and turn her
   
   
Practice 3: Stamp a Pattern
-----------------------------------------------------------

The following blocks can be assembled to draw a circle-like pattern using ``stamp``.

Order Code Here
================

Click on the |start| button below when you are ready to try to order this code.  You will have up to 10 minutes to try to solve it.  Click the |runbutton| button to check your solution.  Click on the |finish| button when you have solved this problem or wish to move on without solving it.

.. timed:: turtle_circle_stamp
   :timelimit: 10
   :noresult:
   :nofeedback:
   :fullwidth:
   
   .. parsonsprob:: inst3_stamp_circle
      :order: 10, 2, 3, 8, 4, 7, 0, 9, 1, 11, 6, 5
      :adaptive:

      The following program uses the stamp method to create a circle of turtle shapes as shown to the left, <img src="./_static/TurtleCircle.png" width="150" align="left" hspace="10" vspace="5"/> but the lines are mixed up.  The program should do all necessary set-up, create the turtle, set the shape to "turtle", and pick up the pen.  Then the turtle should repeat the following ten times: go forward 50 pixels, leave a copy of the turtle at the current position, reverse for 50 pixels, and then turn right 36 degrees.  <br /><br /><p>Drag the needed blocks of statements from the left column to the right column and put them in the right order with the correct indention.  Click on <i>Check Me</i> to see if you are right. You will be told if any of the lines are in the wrong order or are the wrong blocks.</p>  
      -----
      from turtle import *
      space = Screen()
      jose = Turtle()
      =====
      jose.shape("turtle")
      jose.penup()
      =====
      jose.shape("turtle")
      jose.penUp #paired
      =====                   
      for num in range(10):  
      =====                   
      for num in range(10) #paired
      =====    
          jose.forward(50)
      =====
          jose.stamp() 
      =====
          jose.Stamp() #paired  
      =====      
          jose.forward(-50)
      =====      
          jose.forward(-25) #paired
      =====
          jose.right(36)  
      =====
          jose.right(20) #paired           

When you are finished with this problem, or are ready to move on, click the |finish| button and then go to the next page by clicking the right arrow |right| near the bottom right of this page.    
