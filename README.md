# cs-tutoring
Exploring and learning GitHub

#Recursion work with turtles

import turtle

t = turtle.Turtle()
t.speed(30)

def triangle(times, radius, angle, t):
    import math
    if times>0:
        t.up()
        t.right(angle)
        t.goto(0,0)
        t.forward(radius)
        t.right(150)
        t.down()
        sqof_two = math.sqrt(2)
        t.forward(radius * sqof_two)
        t.right(120)
        t.forward(radius * sqof_two)
        t.right(120)
        t.forward(radius * sqof_two)
        t.right(330)

        
            
        triangle(times-1, radius - 10, angle-5, t)
        
triangle(6, 100, 0, t)
