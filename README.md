### @explicitHints true

# Turtle Logo - Lesson #5

## Turtle Logo - Lesson #5 @unplugged
**Making the Turtle's Pen Move Up and Down.**

In this lesson you will make the **Turtle** lift it's pen up and down.
![color](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson5/raw/main/assets/pen_up_screenshot.png)

## Step 1
** Follow Along**

Once again, all our programs begin with an ⇢``on start``⇠ block. Then you need to add the **Turtle** using the ⇢``show turtle``⇠ block.
```blocks
turtle.showTurtle()
```

## Step 2
** Follow Along**

Previously we have learned how to make the **Turtle** move around the game console and leave a trail. But sometimes we might not want to leave a trail, then what?
```blocks
turtle.showTurtle()
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
```

## Step 3
** Follow Along**

To solve this problem you use the ⇢set turtle's pen up⇠ block. As the name implies, it lifts the **Turtle's** pen up
```blocks
turtle.showTurtle()
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.pen(TurtlePenMode.Up)
```

## Step 4
** Follow Along**

Once the pen is up, if you move again no trail will be left behind.
```blocks
turtle.showTurtle()
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.pen(TurtlePenMode.Up)
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
```

## Step 5
** Follow Along**

You can also use the ⇢set turtle's pen up⇠ block again, and change the "up" to "down" to make it leave a trail again.
```blocks
turtle.showTurtle()
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.pen(TurtlePenMode.Up)
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.pen(TurtlePenMode.Down)
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
```
## Step 6
** Try it Out**

Now try moving the **Turtle** some different distances, different directions, turning, changing color and lifting it's pen up and down.
```blocks
turtle.showTurtle()
turtle.setPenColor(8)
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
turtle.pen(TurtlePenMode.Up)
turtle.moveTurtleDirection(TurtleDirection.Forward, 50)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Left, 90)
turtle.setPenColor(7)
turtle.pen(TurtlePenMode.Down)
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
```

## Step 7
**Success!**

You can now change get the **Turtle** to lift the pen up and down.

## Step 8
**Your Turn**

Get your **Turtle** to:
- move
- change its trail color
- turn
- lift the pen up
- move again
- put the pen down
- move again
- then say, "I can lift my pen!"

## Step 9
**Done**

You have successfully completed your fifth lesson in Turtle Logo.

```ghost
turtle.say("Hello, World!")
```
