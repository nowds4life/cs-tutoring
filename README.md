# cs-tutoring
Exploring and learning GitHub

#Recursion work with turtles

import turtle
import math
t = turtle.Turtle()
t.speed(30)

def triangle(times, len, difference, t):
    
    if times>0:
        t.up()
        t.goto(0,0)
        t.right(90)
        threesq = math.sqrt(3)
        t.forward((threesq*(len/2))/2)
        t.right(90)
        t.forward(len/2)
        
        t.down()
        
        t.right(120)
        t.forward(len)
        t.right(120)
        t.forward(len)
        t.right(120)
        t.forward(len)
        t.right(180)
        t.right(difference)
        
        
        
       
        t.down()
            
            
        triangle(times-1, len - len/10, difference, t)
        
triangle(30, 150, 5, t)
