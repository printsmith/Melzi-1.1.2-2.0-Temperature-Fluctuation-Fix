# Read Me!!

**FOREWARNING: This involves soldering and modifying your circuit board. Do this at your own risk, I assumed no responsibility if you mess it up. It involves a small amount of soldering and you should always use safe practices such as using a fume vent or being in a well ventilated area.**

If you're not aware, the Melzi 1.1.2 and 2.0 circuit boards being shipped with the CR-10 and CR-10s have an issue where the temperature sensors cannot reliably read temperatures. This leads to large fluctuations in temperature readings and the thermal runaway protection being triggered, as well as your heater not knowing what to do and trying to correct the bad readings it is getting, further throwing off your temperatures. I did not initially notice the problem when I first started printing with the CR-10 in PLA, I only noticed it when I began trying to print in PETG.

From what I gather, this issue arises from uneven voltage being distributed from the 5V regulator on the Melzi boards. This throws the thermistor readings out of whack since to read temperatures accurately they require a stable voltage being fed into them.  

This issue has been very well documented by independent sources and by TH3D for the V2.0 board, however no one has posted how one can fix their V1.1.2, so this repo will basically document how I fixed mine plus a few other tidbits I leart about the V1.1.2 board. 

**DISCLAIMER: I am in no way affiliated with TH3D, however they are known to be reputable in repairing this issue and are the only ones I know of offering this service**

Preface: I have flashed the bootloader to my board and installed Marlin which I highly suggest everyone do with the Melzi boards given with the Creality 3D printers (I used [this tutorial](http://www.instructables.com/id/Flashing-a-Bootloader-to-the-CR-10/)). I will be uploading my Marlin configurations to this github as well since I've made some changes and even figured out how to get a servo driven Z probe running on this board. 

## How do you know if this problem affects you?

The easiest way to tell if this problem affects you is to check your hotend temperature readings at room temperature. If the readings fluctuate by a few degrees then you most likely have this issue. However, you should tune your PID before and check that all wires are in properly before jumping to any conclusions. TH3D made a very [good little gif](https://i0.wp.com/www.th3dstudio.com/wp-content/uploads/2018/01/2018-01-25_18-22-43.gif?resize=1080%2C607&ssl=1) showing what the flucuations look like.


## I have a CR-10S with a V2.0 board, what do I do?

This issue has been very well documented for the V2.0 board so I will refer you to Jozer99 of Jozerworx and [their tutorial](https://www.jozerworx.com/creality-cr-10s-c4-capacitor-diy-fix-tutorial/) on how to fix it.

And if you don't have the equipment and knowhow to do so, TH3D can fix the issue for you [here](https://www.th3dstudio.com/product/creality-cr-10s-v2-0-board-repair-temperature-fluctuation/).

## I have a CR-10 with a V1.1.2 board, what do I do?

Well as mentioned above, TH3D can fix the V2.0 board as well as the V1.1.2 board so if you're not up for doing it yourself check them out over here: https://www.th3dstudio.com/product/creality-cr-10-v112-board-repair-temperature-fluctuation/

If you want to fix the issue yourself well you're in luck, follow me over [here](https://github.com/tylerkalinowicz/Melzi-1.1.2-2.0-Temperature-Fluctuation-Fix/blob/master/V1.1.2%20Fix/V1.1.2%20Fix%20Tutorial.md) to fix the board yourself!

## Extras

If you want to know how I got a servo Z probe running check it out [here] (I will be adding a little bit on it soon, still in progress).



