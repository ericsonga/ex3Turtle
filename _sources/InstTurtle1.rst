..  Copyright (C)  Mark Guzdial, Barbara Ericson, Briana Morrison
    Permission is granted to copy, distribute and/or modify this document
    under the terms of the GNU Free Documentation License, Version 1.3 or
    any later version published by the Free Software Foundation; with
    Invariant Sections being Forward, Prefaces, and Contributor List,
    no Front-Cover Texts, and no Back-Cover Texts.  A copy of the license
    is included in the section entitled "GNU Free Documentation License".

.. setup for automatic question numbering.

..     qnum::
    :start: 1
    :prefix: 4-1-
    
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

Example 1: Draw Square
------------------------

A turtle in Python automatically starts with its pen down and draws a line as it moves.  The code below will draw a square by
having a turtle turn to face north and then move forward 100 pixels and turn right 90 degrees four times.

Run Code 
=========

Click the |runbutton| button below to see the Turtle draw a square.  

.. activecode:: Turtle_Square
    :nocodelens:
	
    from turtle import *	# use the turtle library
    space = Screen()   		# create a turtle space
    alisha = Turtle()  		# create a turtle named alisha
    alisha.setheading(90)  	# point due north
    for sides in [1,2,3,4]:	# repeat the indented lines 4 times
    	alisha.forward(100)        	# move forward by 100 units
      	alisha.right(90)           	# turn by 90 degrees
   
Practice 1: Draw Rectangle
----------------------------

You can also use a turtle to draw a rectangle.  In a rectangle the opposite sides of the rectangle are the same length.  The code below
can be assembled to draw a rectangle with two opposite sides of length 175 and two opposite sides of length 150.  


Order Code Here
=================

The following code is mixed up and contains extra blocks that are not needed in a correct solution.

Click on the |start| button below when you are ready to try to order this code.  You will have up to 10 minutes to try to solve it.  Click the |checkme| button to check your solution.  Click on the |finish| button when you have solved this problem or wish to move on without solving it.

.. timed:: draw_rect_timed
   :timelimit: 10
   :noresult:
   :nofeedback:
   :fullwidth:
   
   .. parsonsprob:: inst1_draw_rectangle
      :order: 9, 8, 3, 7, 0, 4, 10, 5, 2, 6, 1
      :adaptive:

      The following program uses a turtle to draw a rectangle as shown to the left, <img src="./_static/TurtleRect.png" width="150" align="left" hspace="10" vspace="5" /> but the lines are mixed up. Drag the needed blocks of statements from the left column to the right column and put them in the right order with the correct indention.  There may be additional blocks that are not needed in a correct solution.   Click on <i>Check Me</i> to see if you are right. You will be told if any of the lines are in the wrong order or are the wrong blocks.</p>  
      -----
      from turtle import *      
      =====   
      from Turtle import * #paired     
      ===== 
      space = Screen()
      carlos = Turtle()
      =====
      for i in [1,2]:  
      =====
      for i in [1,2]  #paired
      =====   
          carlos.forward(175)
      =====   
          carlos.Forward(175) #paired
      =====
          carlos.right(90)
      =====
          carlos.left(90) #paired
      =====  
          carlos.forward(150)
          carlos.right(90)
      =====  
          carlos.forward(150)
          carlos.turn(90) #paired
   
When you are finished with this problem, or are ready to move on, click the |finish| button and then go to the next page by clicking the right arrow |right| near the bottom right of this page.    
   
