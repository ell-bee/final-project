# final-project: oscillating ball

## 1. brief description of your idea:
a ball moves back and forth across the screen in a smooth oscillation using sin wave motion.

## 2. describe the things that you are modeling:
i'm modeling one ball that moves left and right based on trigonometric motion. i will create a "ball" class to manage this movement.

## 3. describe the other variables and data structures you'll need:
- one "ball" object
- variables for:
  - "angle" - tracks the current angle used in the sin function
  - "amplitude" - controls how far the ball moves left and right
  - "angularVelocity" - controls how fast the angle changes
- these will be properties inside the "ball" class

## 4. describe what you will do in setup:
- create the canvas
- create the "ball" class
- initialize starting values for angle, amplitude and angular velocity

## 5. describe how the flow of draw will work:
- clear the background
- call "update()" on the ball to change its angle
- call "display()" to draw the ball at its new position
- repeat every frame to create the animation

## 6. describe each of the classes you need in terms of properties and actions:

### "ball" class
**properties:**
- "angle": current angle for sin motion
- "amplitude": how far left/right the ball travels
- "angularVelocity": how fast the angle changes
- "y": vertical position of the ballv (doesn't change)
- "x": calculated using "sin(angle) * amplitude"

**actions:**
- "update()": increases "angle" by "angularVelocity"
- "display()": uses "x" and "y" to draw the ball on the canvas

  
