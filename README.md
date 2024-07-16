# Project Zekrom

This project aims to create an opensource adressable RGB tail for Zekrom and other tech aditions for any Zekrom costume/plush.

## Layout
Due to the large amout of LEDs used there will need to be a large battery pack used.
At the current state I am thinking of using a detachable backpack to power the LEDs.
Other than that, there are no connections or cables ruing outside of each section as they will be powered seperatly and comunicate via a bluetooth network.


## Hardware
Due to the large amount of LEDs used, it is not recomended to use Arduino.
As such, I will be using Raspberry Pi's to control the LEDs and other components.

## LCD Eyes
**ALFA CONCEPT**

LCDs could be used to aimate and miror the wearer's eye movemet with a camera.
Normaly, LCDs are not transparent.
However, removing the backlight and other backig, it is posible to mod an LCD to a trancparent one.
With a ring light you can see out of the LCD, but not see in.
So it looks like firsuit eyes but animated.

## LED Tail
**BETA CONCEPT**

Using standard diffusion techniques and fabric it is posible to mimic Zekrom's overdrive tail.
In this case I will be using 1 inch foam to diffuse the light form the LEDs and coloring it with 50 GSM Black fabric.
Unfortunetly, standard firsuit/plush fabric is too thick to let the light through creating an odd pattern.
If durability is an issue, white 50 GSM fabric can be put under the black fabric, as it lets a lot of light through.
See [Diagram](/Diagram) for more details on the layout and [Examples](/Diagram/Examples) for a demonstration.

As I will be moding a firsuit, I will be getting it with zippers and an inner base for LEDs to be installed on.
The zippers will be located on the bottom of the tail and a circular one will be included to access the flat space.
If you are making it from scrach it does not need zippers; however, it would be uesfull if something needs to be replaced.

The LEDs I will be using is the [Adafruit DotStar Digital LED Strip 60 LED/m](https://www.adafruit.com/product/2240) as
it animates better and has a SPI interface.  Due to the fact that white reflects light, I would recomend using the white version.
I would recomend against the 120 LED/m due to the power required, except perhapse at the tip of the tail.
A 3 section LED controller made to run on the Raspberry Pi will be made at a later date.
As this is a cone, the LEDs will not aline like on a cilinder.

Using other sensors I can start/stop animations based on actions.  Like attacking with the hands, walking, heartbeets, and much more.
Acceleromitors can be used to detect movement and a heart rate sensor installed on the battery backpack can detect the heart rate.

## LED Horn
**BETA CONCEPT**

A smaller strip of RGB LEDs will be used to light up Zekrom's horn with the same concept.
It will however use a [Adafruit DotStar Digital LED Strip 144 LED/m](https://www.adafruit.com/product/2242) so it lights up better.
LED foam may be needed as it is a much tighter space.


## Security
**ALFA CONCEPT**

This is a valuable item, so security is a must.  Tile/Cube trackers can be hidden throughout the body.
NFC tags can be sewn into the suit/plush to provide identification.
A GPS and Celular/LoRa/WiFi moduel can be installed to track and report the position of the main suit/plush.
It will fall back from WiFi to LoRa and Celcular if of range of a public/known network.
The only issue is constant power.  This could be resolved by connecting to the LED battery.  However, if it's removable that is an issue.

## Sensors
Gyrascopes and Acceleromitors can be used to track postions and movemets of the limbs and triger LED animations.
Presure sensors can detect the center of mass.
A heartrate sensor can be usesd to dettect the heartrate ad modify the timing of LEDs.
Flex sensors can be used to detect bends in the hands, though, I don't know what this would be used for.

Ultrasonic distance sensors will not be usable under fabric.  So unfortunetly, they will be obmitted.

Any sensors in the hands, feet, and wings, will be controlled by a Pi Zero 2 as it is not nesisary to have lots of computational power for those sensors.
