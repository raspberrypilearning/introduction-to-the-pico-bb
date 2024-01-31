## RGB LEDs

RGB LEDs produce a range of colours by combining Red(R), Green(G) and Blue(B) light. 

RGB LEDs have 4 legs rather than two. Our projects **common cathode** RGB LEDs which means one leg needs connecting to a **GND** pin and the other three legs need connecting to **GPIO** pins.

<a title="oomlout, CC BY-SA 2.0 &lt;https://creativecommons.org/licenses/by-sa/2.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:RGB_LED.jpg"><img width="512" alt="RGB LED" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f1/RGB_LED.jpg/512px-RGB_LED.jpg"></a>

There are also common anode RGBLEDs, which means that one leg needs connecting to a **3.3V** pin, and the other legs need connecting to **GPIO** pins.

With either type of RGB LED, a resistor is needed for each pin that is connected to a **GPIO** pin. The datasheet for an RGB LED will tell you the **forward current** and **forward voltage** for each colour on the LED, to help you calculate the resistor needed, although it is often easier just to use a fairly high value resistor on each of the legs, such as a 220Ω.

You can prepare your RGB LEDs ready to use in projects:

[[[rgb-led-resistor-electrical-tape]]]

[[[rgb-led-resistor-solder-heat-shrink]]]

Here is how you could wire an RGB LED to a Raspberry Pi Pico.

![Raspberry Pi Pico wired to an RGB LED through GPIO pins 1 - 3 and to GND](images/rgb-led-diagram.png)

[[[rgb-wiring]]]

Set up your RGB LED in your code:

[[[rgb-led-pins]]]

RGB colours can be given using three numbers from 0-255, `(255, 0, 255)` is purple (maximum red and maximum blue). You may need to adjust the colours depending on how bright each of the three colours is for your LED. 

[[[generic-theory-simple-colours]]]

This code makes the LED change between different colours:

--- code ---
---
language: python
filename: main.py
line_numbers: false
line_number_start: 
line_highlights: 
---
from picozero import RGBLED
from time import sleep

rgb = RGBLED(red = 1, green = 2, blue = 3)

while True:
    rgb.color = (255, 0, 0)
    sleep(0.5)
    rgb.color = (0, 255, 0)
    sleep(0.5)
    rgb.color = (0, 0, 255)
    sleep(0.5)
--- /code ---

You can also use `blink`, `pulse` and `cycle` to create colour effects:

[[[pico-rgb-led-blink-pulse-cycle]]]

