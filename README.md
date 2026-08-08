# Pico Calc electronics design
### the electronics portion of an rpi Pico based calculator
## BOM:
| Part name | notes | Qty | Link |
| --- | --- | --- | --- |
| 3.2inch SPI Module ILI9341 SKU:MSP3217 | 3218 will also work as touchscreen is not wired | 1 | https://www.amazon.com/Pasuihcay-240X320-ILI9341-Occupies-MSP3218/dp/B0D5YFC594 |
| 6mm tactile switch |  | 36 | https://www.amazon.com/QTEATAK-Momentary-Tactile-Button-Switch/dp/B07VSNN9S2/ref=sxin_19_pa_sp_search_thematic_sspa?content-id=amzn1.sym.0c718b35-8c59-4938-97bf-b9d1819ea929%3Aamzn1.sym.0c718b35-8c59-4938-97bf-b9d1819ea929&crid=1LEC4S1U00IQO&cv_ct_cx=6mm+switch&keywords=6mm+switch&pd_rd_i=B07VSNN9S2&pd_rd_r=21af0360-bd6d-4493-9a72-96fcb04169b4&pd_rd_w=PqWIq&pd_rd_wg=IrpTp&pf_rd_p=0c718b35-8c59-4938-97bf-b9d1819ea929&pf_rd_r=WY0E907K72MT9R1R7JBZ&qid=1782495894&sbo=RZvfv%2F%2FHxDF%2BO5021pAnSA%3D%3D&sprefix=6mm+switch%2Caps%2C281&sr=1-1-e169343e-09af-4d41-85b1-8335fe8f32d0-spons&aref=jFNKZsthcz&sp_csd=d2lkZ2V0TmFtZT1zcF9zZWFyY2hfdGhlbWF0aWM&psc=1 |
| Pimoroni lipo pico | Note: pico 2 lipo will also work | 1 | https://vilros.com/products/pimoroni-pico-lipo-16mb |
| Lithium Ion Battery - 3.7V 2000mAh | Note: any battery with/connected to a JST-PH connector will work | 1 | https://www.adafruit.com/product/2011 |
| short plug male header | for pico, normal sized header pins and socket will work as well | 2 | https://www.adafruit.com/product/5584 |
| Short Socket Headers | see above | 2 | https://www.adafruit.com/product/5585 |

## design:
The pcb consists of two separated sections, the button matrix and the display connection, connected to an rpi with headers through 2 through hole pin connectors. Buttons are 6mm through hole, display is an MSP321**7** (no touch screen), connector is 1x20 2.54mm. 
**IMPORTANT:** the male header pins should be pointed down for access to bootsel, and the pico's usb port should be pointed outside, to the right if viewed from above.
## software:
see [zig-calc](https://github.com/rod520/zig-calc) for software, and also button overlay.

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
<img width="1498" height="1996" alt="image" src="https://github.com/user-attachments/assets/4190e80a-8c70-449d-8008-b05db41a2d3b" />
