# melzi_creality_temp_fluctuation_fix

If you're not aware, the Melzi 1.1.2 and 2.0 circuit boards being shipped with the CR-10 and CR-10s have an issue where the temperature sensors cannot reliably read temperatures. This leads to large fluctuations in temperature readings and the thermal runaway protection being triggered, as well as your heater not knowing what to do and trying to correct the bad readings it is getting, further throwing off your temperatures. I did not initially notice the problem when I first started printing with the CR-10 in PLA, I only noticed it when I began trying to print in PETG.

Preface, I have flashed the bootloader to my board and installed Marlin which I highly suggest everyone do with the Melzi boards given with the Creality 3D printers (see below for a link to the tutorial I used), I will be uploading my Marlin configurations to this github as well.

## How do you know if this problem effects you?


