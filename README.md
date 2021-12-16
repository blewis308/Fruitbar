# Fruitbar Repository

Here is a comprehensive hub for the Fruitbar Keyboard, designed and written by **Fruit**
<br/>

## Repository Contents:
* firmware
    * everthing firmware related including qmk, zmk, vial, and more!
    * Check out the [QMK Repo](https://github.com/qmk/qmk_firmware/tree/master/keyboards) for big firmware releases.
* open source
    * all the pieces of this board that will be free for use (i.e. plate files, midplate, etc.)
    * *Please note:* if the file does not exist in here, it is not open source and unauthorized copying, distribution, or use of the files via any medium is strictly prohibited.
* img
    * image files for this page.

___

## Table of Contents

* [Prerequisites](#Prerequisites)
* [What's included](#Included)
* [Build guide](#Build)

___

## Prerequisites

There are some items you will need in order to build your Fruitbar

### Required

* Soldering iron
* Solder
* Small phillips screwdriver
* Flush-cutters or wire-cutters

### Optional

* Flux - if you are not using leaded solder, flux is recommended
* Electrical Tape

___

## Included

Included in each kit is the following:
#### Bottom and Switch Plates
![Plates](img/plates.jpg)
#### PCB
![PCB](img/pcb.jpg)
#### Hardware
![Hardware](img/hardware.jpg)
* A - 60 1N4148 Diodes
* B - 16 M2x6mm Screws (+1 extra)
* C - 8 M2x10mm Standoffs
* D - 4 Rubber Feet
* E - 0.91" I2C OLED Module
* F - *Either* Elite-C (Left) or Pro-Micro (Right) - Depends on what you ordered
* G - Holographic Fruitybooty Sticker :)

___

## Build
### Total Estimated Time: 2-3 hours

#### Before you begin!
Please double check everything is here! There is a very slim chance we forgot something or that your order is wrong; in the case this is true, please reach out via email at [support@fruitykeeb.xyz](mailto:support@fruitykeeb.xyz) and we will work with you to get it right. 
**Also**, due to the DIY nature of this hobby, as soon as a soldering iron touches or other modifications happen to the board, I am no longer able to issue a refund/replacement. Please refer to the [terms and conditions](https://www.fruitykeeb.xyz/terms-and-conditions) listed on my site for more info.

Note about this guide: For this guide, I am building a board with an Elite-C and Encoder - yours may differ. You are free to adjust or skip steps if they do not apply to your scenario. 

All that being said, let's get started!

### Step 1: The Diodes
#### Estimated time: 1 hour

The Diode footprints on the PCB are dual-footprint. This means you can use either through-hole (included) or surface-mount diodes on the PCB.

![Diode-Legs](img/diodelegs.jpg)
Bend each diode so the legs are 90deg right next to the diode body.

![Diode-Lines](img/diodelines.jpg)
There is a black line on one end of the diode - when you are putting the diodes into the pcb, make sure you line this up with the filled in side of the marking on the pcb or the way the little arrow is pointing.

![Diode-Example](img/diodeexample.jpg)
This is how it should look, all the diodes should be like this except for the one next to the controller.

![Diode-Solder](img/diodesolder.jpg)
Then solder the diodes in place. [This is a very good video to watch if you are not experienced with through-hole soldering](https://youtu.be/vAx89WhpZ3k). Take your time with this and try not to rush.

<br/><br/>

**Please be careful when cutting the diode legs as the PCB scratches easily and can cause shorts.**


### Step 2: Headers and OLED
#### Estimated time: 30 mins

Before we move on further, we need to solder the headers for the controller and the OLED Module.

*Note:* if you are using peel-a-way or other hotswap sockets for the controller, you may deviate during this step. 

![Controller-Tape](img/controllertape.jpg)
First use tape to hold the headers and controller tight against the PCB

![Controller-Flush](img/controllerflush.jpg)
When we flip the PCB over, we need the headers to be *flush* with the topside of the PCB. This can either be done by adjusting the pins slightly to be flush or by cutting them flush with our flush-cutters from the last step. 

![Controller-Solder](img/controllersolder.jpg)
Then, solder **just the headers to the PCB** **DO NOT solder the controller to the headers yet**!!!

![Oled-Headers](img/oledpins.jpg)
Flip the PCB over and insert the headers for the OLED module and tape in place.

![Oled-Solder](img/oledsolder.jpg)
Solder the OLED headers in place. **Be careful not to let any solder seep into the exposed vias next to the header!** This can cause shorts.

![Oled-Taped](img/oledtape)
Because the OLED needs to rest flush on the PCB, putting a small piece of electrical tape here is **critical**. If this is skipped or excluded, shorts can occur and could render the board in operable. 

![Oled-Soldered](img/oledinstall.jpg)
Now we can install and solder the OLED module as shown and clip the excess from the pins. 


<br/><br/>

### Step 3: Switches and Encoder
#### Estimated time: 1 hour

#### Optional: Encoder
![Encoder-Clip](img/encoderclip.jpg)
First thing we need to do is to clip off the legs on the side of the encoder. These are just for extra support and really serve no function.

![Encoder-Solder](img/encodersolder.jpg)
Next, solder the encoder on in the designated location. 

#### Switches
![Stabilizers](img/stabilizers.jpg)
First up is stabilizers, for this board I'm useing Durock V2 stabs with the full space and full shift layout.

![Switches-Plate](img/switches.jpg)
Next we're going to place a starting amount of switches in our place and press it onto the PCB. I usually recommend 4-10 switches first, but the area around the OLED screen should get all the switches as shown. This helps secure the switches in all the way as the OLED can make the plate bulge a little bit.

