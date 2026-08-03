# Pico Calc electronics design
### the electronics portion of an rpi Pico based calculator

## design:
The pcb consists of two separated sections, the button matrix and the display connection, connected to an rpi with headers through 2 through hole pin connectors. Buttons are 6mm through hole, display is an MSP321**7** (no touch screen), connector is 1x20 2.54mm. 

## software:
todo
## mechanical:
todo


## WHY?
I wanted to make a clone of the numworks calculator, but I realized that wasnt feasible and cheap, so I eventually landed on making a pi-hat like extension for an rpi pico. The pico clone Pimoroni LiPo Pico can connect to  an optional Lithium Ion Battery, so this calculator will (eventually) have nearly every feature of the numworks, albeit with a vertical display, thicker case, and cheap clicky buttons. 

## materials:
1. 36 6mm through hole tactile buttons
2. 2 1x20 female/socket connectors, **2.54 mm**, I'm planning on using Adafruit's short socket headers
3. 2 matching 1x20 male/pin connectors, **2.54 mm**, I'm planning on using Adafruit's short pin headers, or you can stick with the pico's default
4. MSP3217 or MSP3218, both work, but you will not be able to use the MSP3218's touchscreen
5. soldering materials
6. an rpi pico, with headers facing down, (OPTIONAL) pimoroni lipo pico in case you want to use a rechargeable battery
7. (OPTIONAL) a JST-PH battery for the pimoroni lipo pico
## software:
see [zig-calc](https://github.com/rod520/zig-calc) for software
