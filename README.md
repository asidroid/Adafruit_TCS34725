# Adafruit TCS34725 Color Sensor Driver #

This driver is for the Adafruit TCS34725 Breakout.
    ------> http://www.adafruit.com/products/1334

# \usr\local\lib\python3.5\dist-packages\adafruit_tcs34725.py

        def color_rgb_bytes(self):
        r, g, b, clear = self.color_raw
        if r != 0:
            red = int(pow((int((r/clear) * 256) / 255), 2.5) * 255)
            green = int(pow((int((g/clear) * 256) / 255), 2.5) * 255)
            blue = int(pow((int((b/clear) * 256) / 255), 2.5) * 255)
        else:
            red = 0
            green = 0
            blue = 0
        return (red, green, blue)


## About this Driver ##

These modules use I2C to communicate, 2 pins are required to  
interface

Adafruit invests time and resources providing this open source code, 
please support Adafruit and open-source hardware by purchasing 
products from Adafruit!

Written by Kevin (KTOWN) Townsend for Adafruit Industries.
BSD license, check license.txt for more information

All text above must be included in any redistribution

To download. click the ZIP button in the top bar, and check this tutorial
for instructions on how to install: 
http://learn.adafruit.com/adafruit-all-about-arduino-libraries-install-use

