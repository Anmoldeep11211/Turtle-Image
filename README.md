# Turtle-Image
import turtle

def draw_petal(turtle, radius, angle):
    """Draws a single petal using half-circles."""
    turtle.circle(radius, angle)
    turtle.left(180 - angle)
    turtle.circle(radius, angle)
    turtle.left(180 - angle)

def draw_flower():
    window = turtle.Screen()
    window.bgcolor("white")

    flower = turtle.Turtle()
    flower.speed(8)

    # Set the color and start drawing petals
    flower.color("red", "yellow")
    flower.begin_fill()

    # Draw each petal
    number_of_petals = 6
    radius = 100
    angle = 60
    for _ in range(number_of_petals):
        draw_petal(flower, radius, angle)
        flower.left(360 / number_of_petals)

    flower.end_fill()

    # Draw the flower center
    flower.color("orange")
    flower.penup()
    flower.goto(0, -radius//2)
    flower.pendown()
    flower.begin_fill()
    flower.circle(radius//2)
    flower.end_fill()

    flower.hideturtle()
    window.mainloop()

draw_flower()
import turtle

def draw_petal(turtle, radius, angle):
    """Draws a single petal using half-circles."""
    turtle.circle(radius, angle)
    turtle.left(180 - angle)
    turtle.circle(radius, angle)
    turtle.left(180 - angle)

def draw_flower():
    window = turtle.Screen()
    window.bgcolor("white")

    flower = turtle.Turtle()
    flower.speed(8)

    # Set the color and start drawing petals
    flower.color("red", "yellow")
    flower.begin_fill()

    # Draw each petal
    number_of_petals = 6
    radius = 100
    angle = 60
    for _ in range(number_of_petals):
        draw_petal(flower, radius, angle)
        flower.left(360 / number_of_petals)

    flower.end_fill()

    # Draw the flower center
    flower.color("orange")
    flower.penup()
    flower.goto(0, -radius//2)
    flower.pendown()
    flower.begin_fill()
    flower.circle(radius//2)
    flower.end_fill()

    flower.hideturtle()
    window.mainloop()

draw_flower()
