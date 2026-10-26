You may be tempted to try to draw shapes on the Sense HAT's LED matrix by using the `set_pixel` command over and over. However, there is a `set_pixels` command with which you can change all 64 LEDs using one single line of code!
For example, you could draw a Minecraft creeper face on the LED Matrix:

```python
from sense_hat import SenseHat

sense = SenseHat()

# Define some colours
g = (0, 255, 0) # Green
b = (0, 0, 0) # Black

# Set up where each colour will display
creeper_pixels = [
    g, g, g, g, g, g, g, g,
    g, g, g, g, g, g, g, g,
    g, b, b, g, g, b, b, g,
    g, b, b, g, g, b, b, g,
    g, g, g, b, b, g, g, g,
    g, g, b, b, b, b, g, g,
    g, g, b, b, b, b, g, g,
    g, g, b, g, g, b, g, g
]

# Display these colours on the LED matrix
sense.set_pixels(creeper_pixels)
```

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/rpi-sensehat-multiple-pixels-creeper" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>

The Code Editor shows the Sense HAT on its side, so the picture is turned a quarter-turn clockwise. If you see a white smiley face, click **Run** again.

[Open this code in the Code Editor](https://editor.raspberrypi.org/en/projects/rpi-sensehat-multiple-pixels-creeper){:target="_blank"}

You can even use more than two colours, like in this example of Steve from Minecraft:

```python
from sense_hat import SenseHat

sense = SenseHat()

# Define some colours
B = (102, 51, 0)
b = (0, 0, 255)
S = (205,133,63)
W = (255, 255, 255)

# Set up where each colour will display
steve_pixels = [
    B, B, B, B, B, B, B, B,
    B, B, B, B, B, B, B, B,
    B, S, S, S, S, S, S, B,
    S, S, S, S, S, S, S, S,
    S, W, b, S, S, b, W, S,
    S, S, S, B, B, S, S, S,
    S, S, B, S, S, B, S, S,
    S, S, B, B, B, B, S, S
]

# Display these colours on the LED matrix
sense.set_pixels(steve_pixels)
```

<iframe src="https://editor.raspberrypi.org/en/embed/viewer/rpi-sensehat-multiple-pixels-steve" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>

The Code Editor shows the Sense HAT on its side, so the picture is turned a quarter-turn clockwise. If you see a white smiley face, click **Run** again.

[Open this code in the Code Editor](https://editor.raspberrypi.org/en/projects/rpi-sensehat-multiple-pixels-steve){:target="_blank"}
