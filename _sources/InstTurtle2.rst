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
	:prefix: 4-2-
	
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
   
Example 2: Turtle Spirograph
------------------------------------
    
You can use a nested for loop to create repeated patterns with a turtle.  The inner for loop in the code below draws 20 red pentagons and the outer for loop draws a 20 sided green polygon.

.. note ::
   
    To complete a polygon of n sides, use a for loop that repeats n times and turn by 360 / n degrees in each iteration of the loop. The example below draws a 20 sided polygon so it turns 360 / 20 = 18 degrees in the outer loop. The inner loop draws a pentagon with 5 sides so it turns 360 / 5 = 72 degrees each time.
   

Run Code
=========

Click the |runbutton| button to see the spirograph-like pattern that the turtle creates when you use a nested loop.

.. activecode:: Turtle_Spirograph
    :nocodelens:
	
    from turtle import *     # use the turtle library
    from sys import *        # use the system library
    setExecutionLimit(50000) # let this take up to 50 seconds
    space = Screen()         # create a turtle space
    zoe = Turtle()           # create a turtle named zoe
    zoe.setheading(90)       # point zoe due north
    
    for repeats in range(20):   # 20 times to draw the pattern
      	zoe.color("green")      # set the color to green
      	zoe.forward(10)           # Offset the shapes a bit
      	zoe.right(18)             # And turn each one a bit
      	zoe.color("red")          # set the color to red
      
     	# This part makes a pentagon
      	for sides in range(5):    # repeat 5 times
            zoe.forward(50)         # move forward 50 units
            zoe.right(72)           # turn by 72 degrees

   
Practice 2: Spirograph
------------------------------------
   
The code below can be assembled to create a 20 sided blue polygon with the outer loop and 20 red triangles in the inner loop.


Order Code Here
================

Click on the |start| button below when you are ready to try to order this code.  You will have up to 10 minutes to try to solve it.  Click the |runbutton| button to check your solution.  Click on the |finish| button when you have solved this problem or wish to move on without solving it.

.. timed:: spiro2
   :timelimit: 10
   :noresult:
   :nofeedback:
   :fullwidth:
   
   .. parsonsprob:: inst2_turtle_spiro
      :order: 7, 10, 6, 8, 9, 2, 3, 5, 4, 1, 0
      :adaptive:

      There is a way of arranging the statements below such that this image is created. <img src="./_static/RedTrianglesBlueCircle.png" width="200" align="left" hspace="10" vspace="5" /> The turtle will draw many triangles. Move the needed pieces of the program from the left into the space on the right.  Indent lines as needed.
      -----
      from turtle import *
      from sys import *    
      setExecutionLimit(50000) 
      ===== 
      wn = Screen()
      mateo = Turtle()
      mateo.setheading(90)
      ===== 
      wn = Screen()
      mateo = Turtle()
      mateo.setheading(45) #paired
      =====
      for repeats in range(20):
      =====
      for repeats in range(20) #paired
      =====
          mateo.color("blue")
          mateo.forward(10)
          mateo.left(18)
      =====
          mateo.color("blue")
          mateo.forward(10)
          mateo.left(12) #paired
      =====
          for sides in range(3):
      =====
          for sides in range(3) #paired
      =====
              mateo.color("red")
              mateo.forward(50) 
              mateo.right(120)
      =====
              mateo.color("red")
              mateo.forward(50) 
              mateo.right(60) #paired
           

When you are finished with this problem, or are ready to move on, click the |finish| button and then go to the next page by clicking the right arrow |right| near the bottom right of this page.    
