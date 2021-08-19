# Tutorial
```template

basic.forever(function () {
	
})

```

```blocks
basic.showLeds(`
    # # # # #
    # # . # #
    . . . . .
    # . . . #
    . # # # .
    `)
basic.showIcon(IconNames.Heart)
basic.showString("Hello!")
```
## Step 1 @showdialog

Hello!
Today you'll learn to write simple programs using MakeCode. 

## Step 2
A program or an algorithm is a list of operations required to perform a task. These operations are performed one by one, top to bottom.

## Step 3 @showhint

Let's assemble our first program! Find the ``||basic.show string||`` block and add it to your code inside the ``||basic.on start||`` block. Wait for your simulation to begin. Do you see how the Micro:bit executes your command?

```diffblocks
----------
basic.showString("Hello!")
```

## Step 4

Change the code so that the ``||basic.show string||`` block is now inside the ``||basic.forever||`` block. Wait for the simulation to begin and then try to notice the difference. Can you tell what is different now?

```diffblocks
basic.forever(function () {
})
----------
basic.forever(function () {
    basic.showString("Hello!")
})
```


## Step 5
#### Use your imagination!

Now, let's have some fun! Your robot is eager to communicate! Change the text inside the ``||basic.show string||`` block to let it convey it's own message to humanity!

```diffblocks
basic.forever(function () {
})
----------
basic.forever(function () {
basic.showString("Any message here")
})
```

## Step 6
Your robot wants to express its love! Help it do it! Replace the ``||basic.show string||`` block with the ``||basic.show icon||`` block. You can discard blocks that you do not need anymore by dragging them left off the screen.

```diffblocks
basic.forever(function () {
})
----------
basic.forever(function () {
basic.showIcon(IconNames.Heart)
})
```

## Step 7

Let's make the pet's heart pulse. Add one more ``||basic.show icon||`` block to your code and change the icon to a small heart. Do you see the heartbeat?

```diffblocks
basic.forever(function () {
basic.showIcon(IconNames.Heart)
})
----------
basic.forever(function () {
basic.showIcon(IconNames.Heart)
basic.showIcon(IconNames.SmallHeart)
})
```

## Step 8
#### Use your imagination!
Let's make something special! Think of an emotion that a robot being could have and make your robot show it! Use the ``||basic.show leds||`` block from the ``||basic.basic||`` category and click the little squares to turn them on and off. You can make your own animations too!

```diffblocks
basic.forever(function () {
----------
basic.forever(function () {
basic.showLeds(`
    # # # # #
    # # . # #
    . . . . .
    # . . . #
    . # # # .
    `)
})
```
## Step 9
Let's use buttons to run different code sequences! You'll need a ``||input.on button pressed||`` block from the ``||input.input||`` category. This block runs the code inside when you press a specified button. That means you can write several programs and run them with the press of a button!
```block
input.onButtonPressed(Button.A, function () {
	
})
```

## Step 10
Assemble the code as shown to let your robot express two different emotions. Note that we've left the facial expressions for you to fill in – use your own imagination!

When you are finished, run the simulation and click the buttons. Does the robot's face change?

```block
input.onButtonPressed(Button.A, function () {
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
})
input.onButtonPressed(Button.B, function () {
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
})
```
## Step 11
It's time to teach your robot to sing! Look for the ``||music.play melody||`` block inside the ``||music.music||`` blocks category. Here, you can click on the little squares to compose a robot song!

```diffblocks
----------
music.playMelody("B G C5 A D D A G ", 120)
```

## Step 12
#### Use your imagination!
Compose 3 different tunes for your robot to sing: one on start and two for each of the buttons pressed. This time we've deliberately shown you only the part of the program – try to do it by yourself!

```block
input.onButtonPressed(Button.A, function () {
    music.playMelody("B G C5 A D D A G ", 120)
})
```

## Step 13
#### Do it yourself
Use all the things that you`ve learned today to make your robot speak, smile and sing! Write code to use buttons to switch between emotions, songs and phrases. Time to show everyone what you can do!

## Step 14 @showdialog
Micro:bit can do so much more than this with the addition of external electronics: sensors, lights, motors and other fun devices. It can shoot cannons, drive vehicles and play games! 

Feeling interested? Go visit our website:	https://oysterkit.com/craftcode 
