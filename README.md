### @explicitHints true

# Turtle Logo - Lesson #6

## Turtle Logo - Lesson #6 @unplugged
**Making the Turtle's do Loops.**

In this lesson you will learn to use loops, to make your code more efficient.
![loop](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson6/raw/main/assets/looping_screenshot.png)

## Step 1
** Follow Along**

Once again, all our programs begin with an ⇢``on start``⇠ block. Then you need to add the **Turtle** using the ⇢``show turtle``⇠ block.
```blocks
turtle.showTurtle()
```

## Step 2
** Follow Along**

Sometime you might want the **Turtle** to start in a different location and not be in the middle of the screen, say (40, 40). You could use several blocks to: 
- lift the pen up
- move forwards
- turn left
- move forwards
- turn right
- place pen down 

Wow, that is a lot of blocks!
```blocks
turtle.showTurtle()
turtle.pen(TurtlePenMode.Up)
turtle.moveTurtleDirection(TurtleDirection.Forward, 40)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Left, 90)
turtle.moveTurtleDirection(TurtleDirection.Forward, 40)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
turtle.pen(TurtlePenMode.Down)
```

## Step 3
** Follow Along**

There is a block that will just teleport the **Turtle** directly to a new position, say (40, 40) and no trail will be left behind. That is the ⇢``set turtle's position to (x 0, y 0)``⇠ block.

That is way easier!
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(40, 40)
```

## Step 4
** Follow Along**

To move the **Turtle** backwards or down, you use negative numbers. The center of the screen is considered (0, 0).
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(-40, -40)
```

## Step 5
** Follow Along**

You know from previous lessons how to move forwards and then turn 90°.
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(-40, 40)
turtle.moveTurtleDirection(TurtleDirection.Forward, 25)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
```

## Step 6
**Try it out**

If I asked you to draw a square, what would you do?

Pause and try out some solutions.
![color](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson6/raw/main/assets/looping_screenshot.png)

## Step 7
** Follow Along**

Most likely you came up with something like this.
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(-40, 40)
turtle.moveTurtleDirection(TurtleDirection.Forward, 80)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
turtle.moveTurtleDirection(TurtleDirection.Forward, 80)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
turtle.moveTurtleDirection(TurtleDirection.Forward, 80)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
turtle.moveTurtleDirection(TurtleDirection.Forward, 80)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
```

## Step 8
** Did you know**

When you look at the previous solution, you will notice that the same 2 block were repeated 4 times. In programming this is **a really bad idea**. Repeating yourself encourages errors in your code and is hard to change things if needed.
```blocks
turtle.moveTurtleDirection(TurtleDirection.Forward, 80)
turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
```

## Step 9
** Did you know**

What we do instead is use a new block, the ⇢``repeat 4 times, do``⇠ block. It is under the "Loops" menu. 
```blocks
for (let index = 0; index < 4; index++) {
}
```

## Step 10
** Follow Along**

Notice that there is a space inside the block. You can place other blocks in there. Since it has the number "4", any code blocks inside it will be executed 4 times. You can always change the 4 to whatever number you would like. 
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(-40, 40)
for (let index = 0; index < 4; index++) {
}
```

## Step 11
** Follow Along**

So you can now take your 2 blocks that repeated 4 times and place them inside the ⇢``repeat 4 times, do``⇠ block. This produces a much simpler and easier to maintain program. 
```blocks
turtle.showTurtle()
turtle.setPositionCartesian(-40, 40)
for (let index = 0; index < 4; index++) {
    turtle.moveTurtleDirection(TurtleDirection.Forward, 80)
    turtle.turnTurtleDirectionByDegrees(TurtleTurnDirection.Right, 90)
}
```

## Step 12
**Success!**

You can now use loops, to make your code more efficient.

## Step 13
**Your Turn**

Get your **Turtle** to draw a red octagon (a stop sign). Remember in a regular octagon there 8 sides and all the angles are 45°. You might need to decrease the step size and also change the starting position of the **Turtle**, to make the octagon fit the screen.
![octagon](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson6/raw/main/assets/octagon_screenshot.png)

## Step 14
**Done**

You have successfully completed your sixth lesson in Turtle Logo.

```ghost
turtle.say("Hello, World!")
```
